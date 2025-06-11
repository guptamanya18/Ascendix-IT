# Ascendix-IT
📚 AI-Powered Hybrid Recommendation System
A machine learning project that builds a Hybrid Recommender System by combining Collaborative Filtering and Content-Based Filtering to provide personalized book recommendations.

📌 Project Objective
To develop a recommender system that intelligently suggests books based on:

User preferences

Past interactions

Metadata such as book tags/genres

This project compares the performance of:

✅ Collaborative Filtering

✅ Content-Based Filtering

✅ Hybrid Recommender System (combining both)

🧠 Techniques Used
Method	Description
Collaborative Filtering	Based on user-item interaction matrix and cosine similarity between users
Content-Based Filtering	Uses TF-IDF vectors of tags/genres to recommend similar items
Hybrid Model	Weighted combination of collaborative and content-based recommendations

🧰 Tech Stack
Layer	Tool/Library
Language	Python 3.x
Data Handling	Pandas, NumPy
ML & Recommender	Scikit-learn
Visualization	Matplotlib, Seaborn (optional)
UI (optional)	Streamlit / CLI interface

📁 Dataset
Used a custom dataset with the following CSV files:

Books.csv: Contains book IDs, titles, and tags

Ratings.csv: User-book ratings

Tags.csv: Book metadata (used for content features)

📌 Dataset Source: [Provide CSV upload or Kaggle link if public]

🧪 How It Works
1. Data Preprocessing
Load books, ratings, and tags

Merge datasets and clean null/missing values

Create user-item rating matrix

2. Collaborative Filtering
Compute cosine similarity between users

Predict ratings for unrated books

Recommend top N books

3. Content-Based Filtering
Use TfidfVectorizer on book tags

Compute item similarity using cosine similarity

Build user profile and recommend top-matching items

4. Hybrid System
Combine content and collaborative scores

Weight control for tuning effectiveness


🖥️ Interface
Basic CLI: Enter user ID and get top N recommendations

Optional Streamlit UI: Simple dropdown interface for live predictions

🔍 Example Output
text
Copy
Edit
Collaborative Filtering Recommendations for User 8:
Book A, Book B, Book C

Content-Based Recommendations for User 8:
Book X, Book Y, Book Z

Hybrid Recommendations:
Book B, Book X, Book A
📊 Evaluation (Optional)
Compare precision@k or RMSE between:

Collaborative model

Content-based model

Hybrid model

🧠 Learnings
Handling real-world data sparsity

Creating personalized models using vector similarity

Building hybrid systems for better accuracy

