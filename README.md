# Graph RAG on Osedea Blogs

This repository contains two Jupyter notebooks designed for specific tasks: web scraping Osedea blogs and setting up a retrieval-augmented generation (RAG) pipeline with knowledge graphs and vectors.

## Setup

### Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/carllapierre/graph-rag.git
    cd graph-rag
    ```

2. Set up the virtual environment and install dependencies:

    ```sh
    pipenv install
    ```

3. Activate the virtual environment:

    ```sh
    pipenv shell
    ```

4. Start the Jupyter server:

    ```sh
    jupyter notebook
    ```

## Notebooks

### `scraper.ipynb`

- **Purpose**: Scrapes all the blogs from the Osedea website and saves each blog as a PDF in the `./data` directory.
- **Usage**: Open the notebook and run all the cells to start scraping.

### `grag.ipynb`

- **Purpose**: Sets up a retrieval-augmented generation pipeline with knowledge graphs. Indexes data from the `./data` directory and makes it retrievable.
- **Dependencies**: Requires a Neo4j instance and an OpenAI API key. Make sure to fill in these details in the notebook where required.
- **Usage**: Open the notebook, fill in the required details (Neo4j instance DB and OpenAI key), and run all cells. Note that indexing the data can take around 45 minutes.

## Data

- The `./data` directory contains the scraped blog PDFs and is ignored in version control.

