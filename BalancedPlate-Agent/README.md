# BalancedPlate Agent: Reflexion-Driven Nutrition Assistant

BalancedPlate Agent** is an autonomous AI agent designed to help users design balanced, evidence-based meals using only the ingredients available in their pantry. Unlike standard chatbots that might provide generic or potentially inaccurate advice, this agent employs a **Reflexion Loop** to critique, research, and refine its suggestions for clinical and nutritional accuracy.

This project is built as an **Agentic System** using `LangGraph` and `Gemini` to ensure that every nutritional recommendation is grounded in scientific principles and properly cited.

---

### 🛠 How it Works (The Reflexion Loop)

The project follows a 3-step iterative process to ensure high-quality output:

1. **Draft:** The agent generates an initial meal design based on the user's available ingredients.
2. **Execute:** The agent identifies gaps in its reasoning and uses the **Tavily Search API** to fetch real-world nutritional data.
3. **Revise:** The agent synthesizes the search results, critiques its initial draft, and produces a final, evidence-based response with peer-reviewed references.

---

### 🚀 Key Features

* **Agentic Orchestration:** Built with `LangGraph` for robust control flow and state management.
* **Self-Correction:** Uses Pydantic schemas to enforce structured output, forcing the agent to reflect on its own "missing" or "superfluous" information.
* **Evidence-Based:** Connects to external research databases to provide clinical context (e.g., metabolic impact, insulin sensitivity, and lipid profiles).
* **Transparent Reasoning:** Each response includes a "References" section, ensuring full traceability of nutritional claims.

---

### 📁 Project Structure


* `BalancedPlate_Agent.ipynb`: The complete Jupyter Notebook containing the agent logic, tool binding, and the LangGraph graph definition.
* README.md

---

### 🛠 Setup & Installation

1. Clone this repository:
```bash
git clone https://github.com/OmarHKhalil/AI-Agents-Projects.git
cd BalancedPlate-Agent
```


2. Install the required dependencies:
```bash
pip install langchain langgraph langchain-google-genai langchain-community tavily-python pydantic

```


3. Set your API keys in your environment variables:
```bash
export GEMINI_API_KEY="your_gemini_api_key"
export TAVILY_API_KEY="your_tavily_api_key"

```


4. Run the notebook in your preferred environment (Jupyter Lab, VS Code, or Google Colab).

---

### Author

- Developed by: Omar Hafez Khalil
- GitHub: [OmarHKhalil](https://github.com/OmarHKhalil)
- LinkedIn: [Omar Khalil](https://www.linkedin.com/in/omar-khalil-55a674281)