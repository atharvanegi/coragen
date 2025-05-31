# CoRAGen: Comparative Retrieval Augmented Generation

A comparative visualization framework designed for multi-aspect Retrieval Augmented Generation (RAG) that supports analysis across diverse dimensions and perspectives.

**[⬇️ Download this README.md file by clicking the download button in the top-right corner of this artifact]**

## 🌟 Overview

CoRAGen enables users to explore controversial topics and complex questions through a comparative lens, retrieving and presenting evidence from multiple perspectives side-by-side. Built for power users such as students, researchers, lawyers, scientists, and policymakers who require comprehensive analysis and verifiable information.

## 📊 System Architecture

![CoRAGen Pipeline](https://github.com/user-attachments/assets/pipeline-overview.png)

The system follows a comprehensive pipeline from query input through multi-aspect retrieval to summary generation and evaluation, supporting parallel processing across different perspectives.

## ✨ Key Features

### 🔍 Multi-Aspect Retrieval
- Support for multiple search engines (Google, Bing, PyTerrier)
- Aspect-based search with customizable parameters
- Query reformulation and reranking capabilities

### 📝 Comparative Generation
- Side-by-side summary generation across different aspects
- Support for multiple LLM providers (OpenAI, Anthropic, HuggingFace)
- Cross-attribute relevance scoring

### 📊 Advanced Evaluation
- Fine-grained RAG evaluation metrics
- Context relevance, answer relevance, and groundedness scoring
- Cross-aspect relatedness analysis
- LLM-based judges for comprehensive assessment

### ⚙️ Flexible Configuration
- Customizable search engines and algorithms
- Configurable generation models and parameters
- Adjustable evaluation prompts and criteria

## 🖥️ Interface Screenshots

### Main Search Interface
![CRAVE Interface](https://github.com/user-attachments/assets/main-interface.png)
*The main interface showing aspect-based search with "Benefits" and "Drawbacks" comparison*

### Comparative Results Display
![Results Display](https://github.com/user-attachments/assets/results-display.png)
*Side-by-side comparison of summaries with confidence scores and source counts*

### Cross-Aspect Analysis
![Cross-Aspect Analysis](https://github.com/user-attachments/assets/cross-aspect.png)
*Cross-attribute relevance visualization showing relationships between different aspects*

### Detailed Article Analysis
![Article Analysis](https://github.com/user-attachments/assets/article-analysis.png)
*Detailed view with article relevance scores and expandable content*

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- Node.js 14+
- API keys for search engines and LLM providers

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/coragen.git
   cd coragen
   ```

2. **Backend Setup**
   ```bash
   cd Backend/Factchecker
   pip install -r requirements.txt
   ```

3. **Frontend Setup**
   ```bash
   # From root directory
   npm install
   ```

4. **Environment Configuration**
   ```bash
   # Set up environment variables
   export BING_KEY="your_bing_api_key"
   export OPEN-AI-KEY="your_openai_api_key"
   ```

### Running the Application

1. **Start the Backend**
   ```bash
   cd Backend/Factchecker
   python App.py
   ```

2. **Start the Frontend**
   ```bash
   # From root directory
   npm start
   ```

3. **Access the Application**
   - Open your browser to `http://localhost:3000`
   - Backend API runs on `http://localhost:5001`

## 🔧 Configuration

### Search Engines
- **Google**: Web search using Google API
- **Bing**: Web search using Bing API  
- **PyTerrier**: Local search with configurable algorithms (TF-IDF, BM25, colBERT)

### Generation Models
- **OpenAI**: GPT-4, GPT-4 Turbo
- **Anthropic**: Claude 3 Opus, Claude 3 Sonnet
- **HuggingFace**: Custom models with API or local deployment
- **Llama**: Meta's open-source models

### Evaluation Metrics
- **Context Relevance**: How well retrieved content relates to the query
- **Answer Relevance**: How well responses address the original question
- **Groundedness**: How well responses are supported by retrieved evidence
- **Cross-Aspect Relatedness**: Similarity analysis between different perspectives

## 📖 Usage Examples

### Basic Comparative Search
1. Enter your query: "Should LLMs be open sourced?"
2. Add aspects: "Benefits" and "Drawbacks"
3. Configure search engine and generation model
4. Review comparative results with relevance scores

### Advanced Analysis
1. Enable reranking for improved result quality
2. Use cross-aspect comparison to identify overlapping themes
3. Examine individual article relevance scores
4. Export results for further analysis

## 🔬 Research Applications

CoRAGen is designed for various research and professional applications:

- **Academic Research**: Systematic literature review and evidence synthesis
- **Legal Analysis**: Case law comparison and argument development
- **Policy Research**: Multi-stakeholder perspective analysis
- **Journalism**: Fact-checking and balanced reporting
- **Scientific Review**: Hypothesis evaluation across different studies



## 📚 Citation

If you use CoRAGen in your research, please cite our paper:

```bibtex
@article{coragen2024,
  title={CoRAGen: A Comparative User Interface for Multi-Aspect Retrieval Augmented Generation},
  author={Negi, Atharva and Dhole, Kaustubh D. and Agichtein, Eugene},
  journal={arXiv preprint},
  year={2024}
}
```

