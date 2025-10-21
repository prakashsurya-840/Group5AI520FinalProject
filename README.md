# Group5 AAI520 Final Project (Multi-Agent Financial Analysis)

A complete, multi-agent Large Language Model (LLM) system that analyzes a stock (AAPL), downloads prices and news, validates inputs, performs data analysis, visualizes insights, and produces a concise project summary with visuals.

**Course:** AAI-520 (Natural Language Processing & GenAI)  
**Team:** Saman Tavasoli, Andrew Blumhardt, Surya Prakash Kuppa Srinivasan  
**Notebook:** `AI_520_MultiAgentFinancialAnalysisSystem.ipynb`  
**PDF Export:** `AI_520_MultiAgentFinancialAnalysisSystem.pdf`

---

## Project Overview

This project implements an **Agentic AI system** that performs an end-to-end financial analysis workflow.  
The agents work together to analyze Apple’s (AAPL) stock over a defined time range, fetching price data and related news, validating data integrity, running analysis, generating visualizations, and summarizing findings automatically.

---

## System Design – Multi-Agent Roles

- **Orchestrator Agent:** Assigns and coordinates tasks among agents.  
- **Data Agent:** Fetches or loads price and news data for the given date range.  
- **Validation Agent:** Performs data quality checks (missing data, schema validation).  
- **Analysis Agent:** Calculates descriptive statistics, volatility, and trends.  
- **Visualization Agent:** Generates charts and graphs for performance insights.  
- **Evaluation Agent:** Reviews results for logical consistency.  
- **Reporting Agent:** Produces the final project summary and outputs it in readable form.

---

## The Learning Outcomes 

- Understanding of NLP and LLM workflows  
- Application of Agentic AI design principles  
- Integration of multi-agent orchestration and routing  
- Incorporation of data validation, retrieval, and analysis within one notebook  
- Clear visualization and summary generation  
- Use of Hugging Face, Python, and prompt engineering concepts  

---


## Repository Structure

```
Group5AI520FinalProject/
├─ AI_520_MultiAgentFinancialAnalysisSystem.ipynb
├─ AI_520_MultiAgentFinancialAnalysisSystem.pdf
├─ README.md
├─ LICENSE
├─ requirements.txt
├─ agent_memory.json
├─ memory.json
└─ data/
   ├─ AAPL_prices_2025-05-16_2025-10-17.csv
   └─ AAPL_news_2025-05-16_2025-10-17.json

```


---

## Installation & Setup

**Python 3.10+** is recommended.

```bash
# 1. Clone the repository
git clone https://github.com/prakashsurya-840/Group5AI520FinalProject.git
cd Group5AI520FinalProject

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter Notebook
jupyter notebook
```
Then open AI_520_MultiAgentFinancialAnalysisSystem.ipynb and run all cells sequentially.


How It Works

The project executes a multi-agent pipeline that performs automated financial analysis combining stock price and financial news data.

1. Configuration: Define ticker symbol (default: AAPL) and date range.
2. Data Retrieval:
  - The Data Agent loads price data from /data/AAPL_prices_...csv.

  - Loads related financial news from /data/AAPL_news_...json.

3. Validation: The Validation Agent checks for missing values and structure.
4. Analysis: The Analysis Agent computes metrics like average price and volatility.
5. Visualization: The Visualization Agent plots results and summaries.
6. Evaluation: The Evaluation Agent reviews consistency of data and analysis.
7. Reporting: The Reporting Agent prints the final human-readable summary.


Example summary:
```
----------- Step 11: Project Summary -----------
Project: AAI-520 Financial Agent
Team Members: Saman Tavasoli, Andrew Blumhardt, Surya Prakash Kuppa Srinivasan
Analyzed Stock: AAPL
Date Range: 2025-05-16 → 2025-10-17
Price Records Processed: 15
News Items Collected: 0
All workflows (data, validation, analysis, visualization) ran successfully.
```

#### Results & Insights
The project demonstrates full automation using a multi-agent architecture.
Price and news data are both validated and analyzed.
Results are summarized clearly with performance metrics.
The workflow can easily be customized for any stock ticker or date range.
Agents share memory using agent_memory.json and memory.json.


#### Team Roles
- Saman Tavasoli: Workflow design, data pipeline, and summary/report creation
- Andrew Blumhardt: Agent orchestration, validation, and result enhancements
- Surya Prakash Kuppa Srinivasan: GitHub setup, packaging, and final documentation
 for more information.


#### Acknowledgments
University of San Diego – Applied Artificial Intelligence (AAI-520)


#### Key Takeaway
This project demonstrates how Agentic AI can automate and coordinate complex data-driven workflows — integrating stock price analysis with financial news insights to produce consistent, explainable, and human-readable summaries using LLM-based multi-agent collaboration.



