Topic 2: KMP Searching Function
1. What is the purpose?
Suppose we have:
string text = "ABABDABACDABABCABAB";
string pattern = "ABABCABAB";


We need to find where pattern occurs inside text.

Expected output:
Pattern found at index 10


The searching function uses the LPS array that we calculated in the previous function.
2. First understand the function
void KMPSearch(string text, string pattern)

It takes two strings:
- text: The complete string in which we search.
- pattern: The smaller string we want to find.
Now let's understand the code step by step.
3. Step 1: Calculate lengths
int n = text.length();
int m = pattern.length();


Here:
- n = Length of text.
- m = Length of pattern.
For our example:
Text length    = 19
Pattern length = 9


4. Step 2: Create and calculate LPS
vector<int> lps(m, 0);

computeLPS(pattern, lps);


Remember our previous function?

It calculates the LPS array.

For this pattern:
Pattern = ABABCABAB


The LPS array is:
Index:   0 1 2 3 4 5 6 7 8
Pattern: A B A B C A B A B
LPS:     0 0 1 2 0 1 2 3 4


We need this array to handle mismatches.
5. Step 3: Initialize two pointers
int i = 0;
int j = 0;


This is very important.
Pointer	Represents
i	Current index of text
j	Current index of pattern

Imagine two people reading two strings simultaneously.
- Person 1 reads the text using i.
- Person 2 reads the pattern using j.
When characters match, both move forward.
6. Step 4: Start the while loop
while (i < n)


Why i < n?

Because we should continue searching until we reach the end of the text.

Now comes the main logic.
7. Case 1: When characters match
if (text[i] == pattern[j]) {
    i++;
    j++;
}


Let's understand with an example.
Text:    A B A B D A B A C D ...
Pattern: A B A B C


Initially:
i = 0;
j = 0;


Comparison:
text[0]    = A
pattern[0] = A


They match.

Therefore:
i++;  // i = 1
j++;  // j = 1


Next:
text[1]    = B
pattern[1] = B


Again, they match.

Both pointers continue moving.

Eventually:
Text:    A B A B D
Pattern: A B A B C
         ✓ ✓ ✓ ✓ ✗


Four characters matched, but the fifth character does not match.

What should we do now?

This brings us to the most important part.
8. Case 2: When the complete pattern matches
if (j == m) {
    cout << "Pattern found at index " << i - j << endl;

    j = lps[j - 1];
}


What does j == m mean?

Remember:
m = pattern.length();


If j == m, it means every character of the pattern has matched.

For example:
Pattern = ABAB
m = 4

j = 4


Therefore, the pattern is found!

Why i - j?

Suppose:
i = 14
j = 9


The starting index of the matched pattern is:
\[
i-j=14-9=5
\]

Why do we write this?
j = lps[j - 1];


Because we may have another occurrence of the pattern, including an overlapping occurrence.

We use LPS to continue searching without restarting unnecessarily.
9. Case 3: When characters mismatch
This is the heart of KMP searching.
else if (i < n && text[i] != pattern[j]) {
    if (j != 0) {
        j = lps[j - 1];
    }
    else {
        i++;
    }
}


There are two situations.
Situation A: j is not zero
if (j != 0) {
    j = lps[j - 1];
}


Suppose:
Text:    A B A B D
Pattern: A B A B C
         ✓ ✓ ✓ ✓ ✗


Here:
j = 4;


The mismatch happens at D and C.

Now:
j = lps[j - 1];
j = lps[3];
j = 2;


So j becomes 2.

Notice something important:
- i does not change.
- j moves backwards logically using LPS.
- We compare the same text character again with a new pattern character.
Why?

Because we already know that some characters match. We don't need to start matching from the beginning.
Situation B: j is zero
else {
    i++;
}


If j == 0, it means we haven't matched any character of the pattern at the current position.

There is nothing to reuse.

Therefore, simply move to the next text character.

10. Complete searching function
Now combine all three cases.

void KMPSearch(string text, string pattern) {

    int n = text.length();
    int m = pattern.length();

    vector<int> lps(m, 0);

    // Calculate LPS
    computeLPS(pattern, lps);

    int i = 0;  // Text pointer
    int j = 0;  // Pattern pointer

    while (i < n) {

        // Case 1: Characters match
        if (text[i] == pattern[j]) {
            i++;
            j++;
        }

        // Case 2: Complete pattern found
        if (j == m) {
            cout << "Pattern found at index "
                 << i - j << endl;

            j = lps[j - 1];
        }

        // Case 3: Characters mismatch
        else if (i < n && text[i] != pattern[j]) {

            if (j != 0) {
                j = lps[j - 1];
            }
            else {
                i++;
            }
        }
    }
}