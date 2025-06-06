# LangGraph Function Tool Calling Calculator Project

This project demonstrates the integration of LangGraph's function tool calling capabilities to create an intelligent calculator agent. By leveraging LangGraph's graph-based architecture, the agent can interpret natural language inputs, decide when to invoke external tools, and provide accurate computational results.

---

## 🧠 Theoretical Foundations

### What is LangGraph?

LangGraph is a framework designed to build complex, stateful workflows for language models. It allows developers to define nodes (representing tasks or decisions) and edges (representing transitions) to create a directed graph that models the flow of information and actions. This structure is particularly useful for managing multi-step interactions and integrating external tools into language model workflows.

### Understanding Tool Calling

Tool calling enables a language model to decide when to invoke external functions or APIs based on the user's input. In LangGraph, this involves:

1. **Tool Definition**: Creating functions that perform specific tasks (e.g., arithmetic operations) and registering them as tools.
2. **Tool Binding**: Associating these tools with the language model so it knows they are available for use.
3. **Decision Making**: Allowing the model to determine, during runtime, whether a tool should be called to fulfill the user's request.

This approach enhances the model's capabilities by combining its natural language understanding with the precision of external tools.

### Graph-Based Workflow

The project employs a graph-based workflow where each node represents a specific operation:([analyticsvidhya.com][3])

* **Input Node**: Receives and processes the user's natural language query.
* **Decision Node**: Analyzes the query to determine if a tool call is necessary.
* **Tool Node**: If required, invokes the appropriate tool to perform the computation.
* **Output Node**: Presents the result back to the user in a coherent response.([aiproduct.engineer][6])

This modular design ensures clarity in the workflow and facilitates easy debugging and extension.

---

## 🔧 Project Overview

### Objective

To build an intelligent calculator that can interpret natural language queries and perform accurate computations by integrating LangGraph's tool calling features.

### Features

* **Natural Language Processing**: Understands and interprets user queries expressed in everyday language.
* **Dynamic Tool Invocation**: Determines when to call external functions for computations.
* **Accurate Calculations**: Performs precise arithmetic operations using defined tools.
* **Modular Design**: Structured workflow that can be easily extended to include more complex operations or additional tools.

---

## 🧩 Components

### Tool Definitions

Functions are defined to perform basic arithmetic operations such as addition, subtraction, multiplication, and division. These functions are registered as tools within the LangGraph framework, making them available for invocation during the workflow.

### Workflow Graph

The workflow is constructed as a directed graph with the following nodes:([getzep.com][4])

1. **Input Node**: Captures the user's query.
2. **Decision Node**: Analyzes the query to decide if a tool call is necessary.
3. **Tool Node**: Invokes the appropriate arithmetic function if required.
4. **Output Node**: Returns the result to the user.([js.langchain.com][7], [aiproduct.engineer][6])

Edges between these nodes define the flow of data and decisions, ensuring a coherent progression from input to output.

---

## 🚀 Getting Started

### Prerequisites

* Python 3.8 or higher
* Jupyter Notebook
* LangGraph and LangChain libraries([langchain-ai.lang.chat][8], [techcommunity.microsoft.com][9])

### Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/Saim-Hassan786/LangGraph-Function-Tool-Calling-Calculator-Project.git
   cd LangGraph-Function-Tool-Calling-Calculator-Project
   ```



2. **Install Dependencies**:

   ```bash
   pip install -r requirements.txt
   ```



3. **Run the Notebook**:

   Open `LangGraph_Function_Tool_Calling_Calculator_Project.ipynb` in Jupyter Notebook and execute the cells sequentially to see the calculator in action.

---

## 📚 Further Reading

* [LangGraph Documentation](https://python.langchain.com/docs/concepts/tool_calling/)
* [LangChain Tool Calling Guide](https://python.langchain.com/docs/concepts/tool_calling/)
* [LangGraph ReAct Function Calling](https://www.analyticsvidhya.com/blog/2024/10/langgraph-react-function-calling/)
