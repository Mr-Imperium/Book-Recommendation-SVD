# Book Recommendation System

## Project Overview

This project implements a book recommendation system utilizing collaborative filtering techniques. By leveraging the Surprise library, it builds and evaluates a model that provides users with personalized book recommendations based on their past ratings.

## Features

- **Collaborative Filtering**: Utilizes the Singular Value Decomposition (SVD) algorithm to predict book ratings based on users' historical ratings.
- **Model Evaluation**: Calculates the Root Mean Squared Error (RMSE) to assess the model's performance on a test dataset.
- **Personalized Recommendations**: Generates a list of book recommendations for each user based on books they have not yet rated.

## Installation

To run this project locally, follow these steps:

### Prerequisites

Ensure you have the following installed:

- Python 3.x
- pip (Python package installer)

### Install Dependencies

1. Clone the repository and navigate to the project directory:

   ```bash
   git clone https://github.com/your-username/book-recommendation-system.git
   cd book-recommendation-system
   ```

2. Install the required Python packages:

   ```bash
   pip install -r requirements.txt
   ```


## Dataset

The project requires a dataset in CSV format named `book_ratings.csv`, which should include the following columns:

- **User ID**: A unique identifier for each user.
- **ISBN**: The International Standard Book Number (a unique identifier for books).
- **Book Rating**: The rating given by the user, on a scale of 0-10.

Ensure that the `book_ratings.csv` file is placed in the project folder, or adjust the file path in the script as necessary.

## Usage

Once you have installed the dependencies and placed the dataset correctly, you can run the recommendation system.

### Running the Model

To train the model and generate recommendations, execute the following Python script:

```bash
python book_recommendation.py
```

This script will:

1. Load and preprocess the data.
2. Train an SVD model on the ratings data.
3. Evaluate the model's performance using RMSE.
4. Generate book recommendations for a specified user (update the user ID in the code as needed).

### Example Output

Here’s an example of how the recommendations for a user might appear:

```
RMSE on test set: 1.45
Top recommendations for User 1234: [('9780143127741', 8.2), ('9780451531443', 7.9), ...]
```

Feel free to explore and modify the code to enhance its functionality or adapt it to your specific needs!
