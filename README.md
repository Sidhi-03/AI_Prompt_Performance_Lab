# AI Prompt Performance Lab 🧪

A data-driven tool for testing, analyzing, and optimizing AI prompts using Machine Learning evaluation and statistical analysis.

## Overview

AI Prompt Performance Lab helps you scientifically test and optimize your prompts instead of guessing. It combines prompt engineering with ML-based evaluation to provide data-driven insights into prompt effectiveness.

## Features

- **Prompt Experimentation Studio**: Test multiple prompt variations against sample inputs
- **ML Quality Evaluation**: Automated scoring for coherence, relevance, and accuracy
- **Statistical Analysis**: Compare prompt performance using pandas/numpy analytics
- **Pattern Library**: Scikit-learn clustering to identify successful prompt patterns
- **Cost Analysis**: Track token usage and estimate costs across variations
- **Visualizations**: Interactive charts showing prompt effectiveness metrics
- **CSV Export**: Export experiment results for further analysis

## Tech Stack

- **Backend**: Python, FastAPI
- **AI Integration**: OpenAI API
- **Data Analysis**: Pandas, NumPy
- **Machine Learning**: Scikit-learn
- **Visualization**: Chart.js, Plotly
- **Frontend**: HTML, CSS, JavaScript

## Project Structure

```
prompt-performance-lab/
├── src/
│   ├── api/
│   │   ├── __init__.py
│   │   ├── routes.py          # API endpoints
│   │   └── models.py          # Pydantic models
│   ├── core/
│   │   ├── __init__.py
│   │   ├── prompt_engine.py   # Prompt testing logic
│   │   ├── evaluator.py       # ML-based evaluation
│   │   └── analyzer.py        # Statistical analysis
│   ├── ml/
│   │   ├── __init__.py
│   │   ├── quality_scorer.py  # Quality scoring models
│   │   └── pattern_cluster.py # Prompt pattern clustering
│   ├── utils/
│   │   ├── __init__.py
│   │   ├── openai_client.py   # OpenAI API wrapper
│   │   └── helpers.py         # Utility functions
│   └── __init__.py
├── static/
│   ├── css/
│   │   └── styles.css
│   └── js/
│       └── app.js
├── templates/
│   └── index.html
├── data/
│   ├── experiments/           # Saved experiments
│   └── exports/               # CSV exports
├── main.py                    # Application entry point
├── requirements.txt           # Python dependencies
├── .gitignore
└── README.md
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/prompt-performance-lab.git
cd prompt-performance-lab
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
```bash
export OPENAI_API_KEY="your-api-key-here"
```

4. Run the application:
```bash
python main.py
```

5. Open your browser and navigate to `http://localhost:5000`

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/` | Web interface |
| POST | `/api/experiments` | Create new experiment |
| GET | `/api/experiments` | List all experiments |
| GET | `/api/experiments/{id}` | Get experiment details |
| POST | `/api/experiments/{id}/run` | Run prompt tests |
| GET | `/api/experiments/{id}/analyze` | Get statistical analysis |
| GET | `/api/experiments/{id}/export` | Export results to CSV |
| GET | `/api/patterns` | Get prompt pattern clusters |

## Usage Example

1. **Create an Experiment**: Define your task (e.g., "summarize articles")
2. **Add Prompt Variations**: Create multiple prompts to test
3. **Provide Test Inputs**: Add sample data to test against
4. **Run Experiment**: Execute all prompts against test inputs
5. **Analyze Results**: View ML-scored quality metrics
6. **Export Data**: Download CSV for detailed analysis

## Skills Demonstrated

- **Prompt Engineering**: Systematic approach to prompt optimization
- **Machine Learning**: Classification and clustering for evaluation
- **Python/Pandas**: Data analysis of prompt performance
- **NumPy/Scikit-learn**: Statistical analysis and ML models
- **Data Visualization**: Charts showing prompt effectiveness
- **API Development**: RESTful API design with FastAPI

## License

MIT License

## Author

Built as a portfolio project demonstrating AI/ML fundamentals and prompt engineering skills.