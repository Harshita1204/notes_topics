# Large Language Models (LLMs)

## Definition
Large Language Models are deep learning models trained on massive text datasets to understand and generate human language.

Examples:
- GPT
- LLaMA
- Claude

LLMs are based on the **Transformer architecture**.

---

# Transformer Architecture

Transformers process entire sequences at once using **attention mechanisms**.

Components:

Encoder
Decoder

Encoder processes input text.
Decoder generates output text.

Example use:
Machine translation.

---

# Tokenization

Computers cannot process raw text.

Text must be converted into tokens.

Example:

Sentence:
"I love AI"

Tokens:
[I] [love] [AI]

Each token is mapped to a number.

Example:
I → 21  
love → 103  
AI → 456

---

# Embeddings

Tokens are converted into vectors.

Example:

king → [0.23, -0.11, 0.78]

Embeddings represent semantic meaning.

Example relationship:

king − man + woman ≈ queen

---

# Attention Mechanism

Attention determines which words in a sentence are most important.

Example:

"The animal didn't cross the road because it was tired."

Attention helps model know **"it" refers to animal**.

---

# Self Attention

Each word examines other words in the same sentence.

Example:

"The cat sat on the mat"

The word "sat" attends to "cat".

This helps understand context.

---

# Pretraining

LLMs are trained on large internet datasets.

Training objective:

Predict missing words.

Example:

"The capital of France is ___"

Correct prediction: Paris.

---

# Fine Tuning

After pretraining, models are specialized for tasks.

Examples:

Chatbots  
Code generation  
Medical assistants

---

# Inference

Inference is when a trained model generates output.

Steps:

1. Prompt tokenized
2. Converted to embeddings
3. Passed through transformer layers
4. Model predicts next token

---

# Prompt Engineering

Prompt engineering improves output quality.

Example:

Bad prompt:
Explain ML

Better prompt:
Explain machine learning with simple examples.

Advanced prompts:

Few-shot prompting  
Chain-of-thought prompting

---

# Vector Databases

LLM systems store embeddings in vector databases.

Example flow:

Document → Embedding → Vector Database

Query → Embedding → Similarity Search

Common vector databases:

Pinecone  
Weaviate  
Milvus