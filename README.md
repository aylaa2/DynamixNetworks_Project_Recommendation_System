# DynamixNetworks_Project_Recommendation_System 

##  Overview
This repository contains the code for **Task 2: Recommendation System**, completed as part of the Machine Learning Internship at **Dynamix Networks**.

The project implements an **Item-Based Collaborative Filtering** system using Python and Pandas. It analyzes user ratings from the MovieLens dataset to suggest movies that are statistically similar to a user's selection.

## Key Features
* **Data Processing:** Merges and cleans `movies.csv` and `ratings.csv` to create a usable dataset.
* **User-Item Matrix:** Converts raw data into a pivot table for analysis.
* **Correlation Engine:** Uses statistical correlation (Pearson) to find similarities between movie ratings.
* **Smart Filtering:** Removes movies with fewer than 50 ratings to avoid noise and ensure quality recommendations.
* **Interactive System:** Users can input any movie title (e.g., "Toy Story (1995)") and receive top 10 recommendations.

## Tech Stack
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy
* **Environment:** Google Colab / Jupyter Notebook

##  Dataset
The project uses the **MovieLens Latest Small** dataset provided by GroupLens Research.
* `movies.csv`: Contains Movie IDs and Titles.
* `ratings.csv`: Contains User IDs, Movie IDs, and Ratings (0.5 - 5.0).
* *Source:* [GroupLens MovieLens Datasets](https://grouplens.org/datasets/movielens/)

##  Results Demo
When the user searches for **"Toy Story (1995)"**, the system recommends:

| Rank | Movie Title | Correlation |
| :--- | :--- | :--- |
| 1 | Toy Story (1995) | 1.000 |
| 2 | Toy Story 2 (1999) | 0.699 |
| 3 | The Incredibles (2004) | 0.643 |
| 4 | Finding Nemo (2003) | 0.618 |
| 5 | Aladdin (1992) | 0.611 |

*(As seen in the output, the system successfully identifies other popular animations and Pixar films.)*

##  How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/DynamixNetworks_Project_Recommendation_System.git](https://github.com/aylaa2/DynamixNetworks_Project_Recommendation_System.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy
    ```
3.  **Run the Notebook:**
    Open `Movie_Recommendation_System.ipynb` in Jupyter Notebook or Google Colab and run all cells.

##  Author
**[Ayla Zeitouni]**
* **Internship:** Machine Learning Intern at Dynamix Networks
* **Task:** Task 2 (Recommendation System)
* **Date:** Feb 2026

---
*Submitted for the Dynamix Networks Internship Program.*
