# 🧠 LangChain Tools & Agent Learning Repository

This repository contains my hands-on learning and implementation of **LangChain Tools** and how they are used within **Agents**.

---

## 🚀 Overview

In this project, I explored how tools enhance the capabilities of LLM-based agents by allowing them to:

* Interact with external systems
* Perform computations
* Execute commands
* Fetch real-time information

This repo demonstrates both **built-in tools** and **custom tool creation** using LangChain.

---

## 🧩 What I Learned

### 🔹 1. What are Tools in LangChain?

Tools are functions that an **agent can call** to perform specific tasks.

Instead of relying only on LLM reasoning, tools allow agents to:

* Execute code
* Query APIs
* Perform calculations
* Access real-world data

---

### 🔹 2. Tools in Agents

Agents use tools dynamically based on the query.

For example:

* If user asks for math → agent calls calculator tool
* If user asks for search → agent calls search tool

This makes agents **more powerful and autonomous**.

---

## 🛠️ Built-in Tools Implemented

### 🌐 DuckDuckGo Search Tool

* Used for real-time information retrieval
* Helps agent answer questions beyond training data

### 💻 Shell Tool

* Allows execution of system commands
* Demonstrates interaction with OS-level operations

---

## ⚙️ Custom Tools Implemented

I implemented multiple custom tools using different approaches:

---

### 🔸 1. `@tool` Decorator

Simple way to convert Python functions into tools.

#### Example:

```python
@tool
def add(a: int, b: int) -> int:
    return a + b
```

---

### 🔸 2. Structured Tool

* Allows defining input schema
* Better control over arguments

Used for:

* Add
* Multiply

---

### 🔸 3. BaseTool (Advanced)

* Full control over tool behavior
* Custom logic and validation

Used to implement:

* Addition
* Multiplication


---

## 🧮 Custom Math Toolkit

I also created a **custom toolkit** that groups multiple tools together.

### 🔹 MathToolkit Features:

* Add function
* Divide function

This demonstrates how multiple tools can be packaged into a reusable toolkit.

---

```

---

## 🎯 Key Takeaways

* Tools are essential for building **real-world AI agents**
* Agents + Tools = **Actionable AI systems**
* Custom tools provide flexibility beyond built-in ones
* Toolkits help organize and scale tool usage

---

## 📌 Future Improvements

* Add API-based tools (weather, finance, etc.)
* Integrate tools with real-world applications
* Build multi-tool intelligent agents
* Add memory + tool combination

---

## 🙌 Conclusion

This project helped me understand:

* How tools work internally in LangChain
* How agents decide which tool to use
* How to build and organize custom tools

It’s a foundational step toward building **production-level AI agents**.

---


