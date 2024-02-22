# phrase-ticker Dataset Generator

The phrase-ticker Dataset Generator is a Python project, designed to link S&P 500 company tickers with relevant natural language phrases. Utilizing GPT-4, this tool aims to enhance stock ticker extraction from textual data, supporting financial NLP tasks like sentiment analysis and entity recognition. It's crafted for easy integration with the Hugging Face `datasets` library, making it an invaluable asset for machine learning applications in finance.

## Contents

- **Data Collection**: Utilizes web scraping to gather names and ticker symbols of S&P 500 companies from Wikipedia.
- **Phrase Generation**: Employs GPT-4 to generate natural language phrases related to each company.
- **Dataset Construction**: Assembles the generated phrases and tickers into a structured dataset.
- **Hugging Face Integration**: Formats the dataset for seamless use with the Hugging Face `datasets` library.

## Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook or JupyterLab
- Pip for package installation

### Installation

1. Clone the repository:
   ```sh
   git clone git@github.com:rohanmahen/phrase-ticker.git
   ```
2. Navigate to the project directory:
   ```sh
   cd phrase-ticker
   ```
3. Install required Python packages:
   ```sh
   pip install -r requirements.txt
   ```

### Configuration

Ensure your environment is correctly set up:

1. Sign up at [OpenAI](https://openai.com/) to obtain an API key.
2. In the project root, create a `.env` file and insert your OpenAI API key:
   ```
   OPENAI_API_KEY='your_api_key_here'
   ```
   **Important:** To secure your API key, do not share or commit the `.env` file.

### Usage

Open and run the `src/main.ipynb` notebook to generate the dataset:

```sh
jupyter notebook src/main.ipynb
```

or

```sh
jupyter lab src/main.ipynb
```

Follow the notebook instructions for detailed steps on data collection, phrase generation, dataset construction, and export.



## Contributing & Usage

We welcome contributions! Feel free to fork the repository and submit pull requests with enhancements, bug fixes, or documentation improvements. Also please feel free to use the dataset for your own projects via [HuggingFace](https://huggingface.co/datasets/rohanmahen/phrase-ticker).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
