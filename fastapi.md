# FastAPI

## Definition

FastAPI is a modern Python web framework for building APIs.

It is known for high performance and automatic documentation.

---

# Key Features

Fast execution  
Async support  
Automatic API documentation  
Type safety

---

# Example

from fastapi import FastAPI

app = FastAPI()

@app.get("/")
def home():
    return {"message": "Hello World"}

---

# Advantages

High performance  
Easy to use  
Built-in validation  
Automatic docs with Swagger

---

# Use Cases

Machine learning APIs  
Microservices  
Backend services