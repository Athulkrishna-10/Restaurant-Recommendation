# Restaurant Recommendation System

### Overview
This project implements a restaurant recommendation system in Google Colab using Python. It uses machine learning to recommend restaurants based on cuisines, ratings, cost, and features like table booking and online delivery. The system employs TF-IDF vectorization for cuisines and cosine similarity for recommendations.
Features

Data Preprocessing: Cleans missing data and encodes categorical variables (e.g., City, Table Booking, Online Delivery).
Feature Engineering: Combines numerical features (ratings, cost, votes) with TF-IDF cuisine vectors.
Recommendation Engine: Recommends similar restaurants using cosine similarity.
Colab-Friendly: Designed to run seamlessly in Google Colab.

### Setup in Google Colab

Open in Colab:
Upload the script (restaurant_recommender.py) and dataset (Dataset.csv) to your Google Drive or directly to Colab.
Alternatively, clone the repository:!git clone https://github.com/your-username/restaurant-recommendation-system.git




Install Dependencies:Run the following in a Colab cell:!pip install pandas numpy scikit-learn


Load Dataset:
Ensure Dataset.csv is in the /content/ directory or update the file path in the script:file_path = '/content/Dataset.csv'


Upload the dataset via Colab’s file upload or mount Google Drive:from google.colab import drive
drive.mount('/content/drive')





### Usage

Run the script in Colab:
Copy the code into a Colab notebook or run the .py file.


Test the recommendation system:recommendations = recommend_restaurants('Le Petit Souffle', top_n=5)
print(recommendations)

This outputs the top 5 restaurants similar to "Le Petit Souffle" based on features like cuisines and ratings.



### Example Output
For Le Petit Souffle:
   Restaurant Name          Cuisines  Aggregate rating  Average Cost for two  Votes
0  Restaurant A     Italian, Continental             4.2                  1500    120
1  Restaurant B     French, Italian               4.1                  1400    100
...

### Contributing
Contributions are welcome! Submit a pull request or open an issue on GitHub to suggest improvements or report bugs.
Credits
Developed by Athulkrishna.KS.
License
MIT License.
