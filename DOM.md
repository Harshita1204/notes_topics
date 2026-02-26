# DOM (Document Object Model)

---

# Definition

DOM (Document Object Model) is a programming interface 
that represents an HTML or XML document as a tree structure.

Each HTML element becomes a node in the tree.

It allows JavaScript to:

- Read content
- Modify content
- Add/remove elements
- Change styles
- Handle events

---

# DOM Tree Structure

Example HTML:

<html>
  <body>
    <h1>Hello</h1>
    <p>World</p>
  </body>
</html>

Converted into:

Document
 └── html
      └── body
           ├── h1
           └── p

Each element = Node
Each attribute = Property

---

# Types of Nodes

1. Document Node
2. Element Node
3. Text Node
4. Attribute Node
5. Comment Node

---

# How Browser Uses DOM

Browser Rendering Pipeline:

1. Parse HTML → Create DOM Tree
2. Parse CSS → Create CSSOM Tree
3. Combine → Render Tree
4. Layout (Reflow)
5. Paint
6. Composite

DOM is central to rendering.

---

# DOM Manipulation Example

Select element:
document.getElementById("id")

Change content:
element.innerHTML = "New Content"

Add element:
document.createElement()

Remove element:
element.remove()

---

# Why DOM Operations Are Expensive

DOM lives inside browser engine.

When DOM changes:

- Reflow may trigger
- Repaint may trigger
- Layout recalculation happens

Frequent DOM manipulation reduces performance.

---

# Reflow vs Repaint

Reflow:
Layout recalculation
Example: Changing width, height

Repaint:
Visual update without layout change
Example: Changing color

Reflow is more expensive than repaint.

---

# Event Propagation

DOM follows 3 phases:

1. Capturing Phase
2. Target Phase
3. Bubbling Phase

Event bubbling is commonly used.

Example:
Click on button → event bubbles to parent.

---

# DOM vs Virtual DOM

Real DOM:
- Direct browser representation
- Slow updates
- Triggers reflow

Virtual DOM:
- JS object representation
- Diffing algorithm
- Batched updates

---

# Performance Best Practices

1. Minimize direct DOM updates
2. Batch changes
3. Use document fragments
4. Avoid forced synchronous layout
5. Use requestAnimationFrame for animations

---

# Memory Consideration

Large DOM trees:

- Increase memory usage
- Slow rendering
- Increase layout time

Keep DOM shallow and optimized.

