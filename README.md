# Chess Games Win Likelihood Prediction

## About the Project
**Chess Games Win Likelihood Prediction** explores the fascinating world of chess, a game of strategy and skill that has thrived since the 15th century. Our project delves into the analytics of chess, focusing on two key factors that potentially influence the outcome of a game: the **type of opening played** and the **players' Elo rating differential**.

Chess games are typically structured into three stages: the opening, the midgame, and the endgame. Among these, the opening moves are based on established patterns, each with its unique name and strategic implications. Additionally, the Elo rating system provides a standardized measure of a player's skill, ranging from 200 to 2800. This rating system calculates win probabilities based on the players' relative skill levels, represented by their Elo ratings.

In this project, we analyze a dataset of approximately 6 million chess games played on Lichess, a popular online chess platform, during July 2016. We want to answer the following question: What better predicts the likelihood of winning a chess game - the opening strategy employed, the difference in Elo ratings between the players, or a combination of both?

This analysis aims to provide insights into the relative impact of these factors on game outcomes, offering a data-driven perspective to the ongoing debate among players and enthusiasts about the effectiveness of different chess openings and the role of player skill in determining game results.

## Installation and Setup
### Prerequisites
* **Python** 3.8 or higher.
* **Anaconda**. [Download Anaconda](https://www.anaconda.com/download). This project uses several packages that are conveniently available through Anaconda. Alternatively, you can use pip to install the necessary packages.
* **Jupyter Notebook** for running .ipynb files. It comes pre-installed with Anaconda, or you can install it separately if using pip:
  ```bash
  pip install notebook
  ```
* **Required Python Libraries**:
  * requests: For making HTTP requests.
  * beautifulsoup4: For web scraping.
  * pandas: For data manipulation and analysis.
  * numpy: For numerical computing.
  * seaborn and matplotlib: For data visualization.
  * scikit-learn: For machine learning models and utilities.
  * scipy: For scientific computing.
  * statsmodels: For statistical modeling.
    * With Anaconda, you can install these packages using:
      ```bash
      conda install requests beautifulsoup4 pandas numpy seaborn matplotlib scikit-learn scipy statsmodels
      ```
    * If using pip, the libraries can be installed via:
      ```bash
      pip install requests beautifulsoup4 pandas numpy seaborn matplotlib scikit-learn scipy statsmodels
      ```
* **SQL Magic and DuckDB**:
  * SQL magic is used for database operations within Jupyter notebooks, and DuckDB is an in-memory SQL database used in this project.
    * Install them using Anaconda:
      ```bash
      conda install -c conda-forge ipython-sql duckdb
      ```
    * Alternatively, they can installed using pip:
      ```bash
      pip install ipython-sql duckdb
      ```
* **Setting Up a Virtual Environment (Optional but Recommended)**
  * To prevent potential conflicts with other Python projects or system-wide packages, consider using a virtual environment.
    * With Anaconda, create a new environment like this:
      ```bash
      conda create -n myenv python=3.8
      conda activate myenv
      ```
    * Install the necessary packages in this environment.

### Cloning the Repository
To get started with the project, you first need to clone the repository to your local machine. Follow these steps:
1. **Open Your Terminal or Command Line:** This can be the Terminal app on macOS or Linux, Command Prompt or PowerShell on Windows, or any other terminal application you prefer.
2. **Clone the Repository:** Run the following command.
   ```bash
   git clone https://github.com/jeanie-liu/chess_win_predictor.git
   ```
3. **Navigate to the Project Directory:** After cloning, move into the project directory with this command:
   ```bash
   cd chess_win_predictor
   ```
With the repository cloned and ready, you can proceed with the installation of the project dependencies as outlined in the prerequisites.

## Usage

This project consists of two main Jupyter notebooks:

1. **Data Cleaning (`data_cleaning.ipynb`):**
   - Download the required raw chess games dataset from Kaggle: [Chess Games Dataset](https://www.kaggle.com/datasets/arevel/chess-games).
   - Place the downloaded dataset in the same directory as `data_cleaning.ipynb` or adjust the file path within the notebook accordingly.
   - This notebook processes the raw data into `chess_games_cleaned.csv`. To view or run the data cleaning process, open `data_cleaning.ipynb` in Jupyter Notebook or JupyterLab.

2. **Analysis and Reporting (`chess_win_likelihood_prediction_report.ipynb`):**
   - This notebook uses `chess_games_cleaned.csv` from the `data` folder.
   - You can use the provided `chess_games_cleaned.csv` in the `data` folder or generate it by running the `data_cleaning.ipynb` notebook. Ensure the file is correctly named and located.
   - Open `chess_win_likelihood_prediction_report.ipynb` to either view the analysis and findings or run the notebook for a more interactive experience.

To work with these notebooks:

- Launch Jupyter Notebook or JupyterLab.
- Navigate to the directory containing the project files.
- Open the notebook of your choice (`data_cleaning.ipynb` or `chess_win_likelihood_prediction_report.ipynb`).
- You can either run the cells to execute the code or simply review the content and findings.




 
