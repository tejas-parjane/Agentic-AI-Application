# Agentic AI Application

A multi-agent system for financial analysis and web research using AI agents powered by Groq and OpenAI models.

## 📁 Project Structure

```
Agentic-ai-application/
├── basic-agents/
│   └── multiagent.py
└── financial-agents/
    ├── financial_analyst.py
    └── playground.py
```

## 🌟 Features

- **Multi-Agent Collaboration**: Specialized agents working together for comprehensive analysis
- **Web Search Agent**: Real-time information retrieval from the web
- **Finance Agent**: Stock analysis, company fundamentals, and analyst recommendations
- **Interactive Playground**: Visual interface for agent interaction
- **Dual Framework Support**: Implementations using both `agno` and `phi` frameworks

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- API Keys:
  - Groq API Key
  - OpenAI API Key (for playground)
  - Phi API Key (for playground interface)

### Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd Agentic-ai-application
```

2. Install dependencies for basic agents:
```bash
cd basic-agents
pip install -r requirements.txt
```

3. Install dependencies for financial agents:
```bash
cd ../financial-agents
pip install -r requirements.txt
```

4. Create a `.env` file in the root directory:
```env
GROQ_API_KEY=your_groq_api_key
OPENAI_API_KEY=your_openai_api_key
PHI_API_KEY=your_phi_api_key
```

## 📦 Dependencies

### Basic Agents
- agno
- openai
- groq
- python-dotenv
- duckduckgo-search
- pypdf
- lancedb
- streamlit
- pandas
- tantivy
- yfinance

### Financial Agents
- phidata
- python-dotenv
- yfinance
- packaging
- duckduckgo-search
- fastapi
- uvicorn
- groq
- openai
- sqlalchemy
- pgvector
- psycopg[binary]
- pypdf

## 💻 Usage

### Basic Agents (Agno Framework)

Run the multi-agent system to analyze stocks:

```bash
cd basic-agents
python multiagent.py
```

**Example Output**: Analyzes Tesla, NVIDIA, and Apple stocks to provide investment recommendations.

### Financial Agents (Phi Framework)

#### 1. Financial Analyst

```bash
cd financial-agents
python financial_analyst.py
```

**Features**:
- Analyst recommendations
- Latest company news
- Stock fundamentals
- Real-time data visualization

#### 2. Interactive Playground

```bash
cd financial-agents
python playground.py
```

Access the playground at `http://localhost:7777` for an interactive interface.

## 🤖 Agent Capabilities

### Web Search Agent
- Real-time web information retrieval
- Source citation
- Powered by DuckDuckGo

### Finance Agent
- Stock price tracking
- Analyst recommendations
- Company fundamentals
- Latest financial news
- Tabular data presentation

### Multi-Agent Team
- Collaborative analysis
- Combined web and financial insights
- Comprehensive investment recommendations

## 🔧 Configuration

Both implementations use environment variables for API key management. Ensure your `.env` file contains:

```env
GROQ_API_KEY=<your-key>
OPENAI_API_KEY=<your-key>
PHI_API_KEY=<your-key>
```

## 📊 Example Queries

- "Analyze companies like Tesla, NVIDIA, Apple and suggest which stock to buy for longterm investment"
- "Summarize analyst recommendations and share the latest news for NVDA"
- "Get stock fundamentals for AAPL"
- "What are the latest developments in AI companies?"

## 🛠️ Models Used

- **Groq Models**:
  - `qwen-2.5-32b`
  - `llama-3.3-70b-versatile`
  - `llama3-groq-70b-8192-tool-use-preview`
  - `llama-3.1-70b-versatile`

## 📝 Notes

- Agents display tool calls for transparency
- Data is presented in markdown format
- Tables are used for structured financial data
- Sources are always included in responses

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.


## 🔗 Links

- [Agno Documentation](https://docs.agno.com)
- [Phidata Documentation](https://docs.phidata.com)
- [Groq API](https://groq.com)

## ⚠️ Disclaimer

This tool is for educational and research purposes only. Always conduct your own research and consult with financial advisors before making investment decisions.

---

**Built with ❤️ using Agno and Phidata frameworks**
