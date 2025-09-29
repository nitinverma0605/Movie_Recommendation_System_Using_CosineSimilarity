# Movie Recommendation System 🎬  

## Overview  
This project builds a **content-based movie recommendation system** using the **TMDB 5000 Movies Dataset**.  
The system recommends similar movies based on metadata such as genres, keywords, cast, and crew.  

The project demonstrates skills in:  
- Data cleaning and preprocessing  
- Feature engineering (text parsing and transformation)  
- Natural Language Processing techniques (bag-of-words, cosine similarity)  
- Building a recommendation function  

---

## Dataset  
The dataset comes from [TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) and includes:  
- **tmdb_5000_movies.csv** – Movie details like genres, keywords, overview  
- **tmdb_5000_credits.csv** – Cast and crew information  

---

## Workflow  
1. **Load Data**: Import and merge `movies.csv` and `credits.csv`  
2. **Preprocessing**:  
   - Extract and clean genres, keywords, cast, and crew  
   - Handle missing values  
   - Normalize text features  
3. **Feature Engineering**:  
   - Create a combined "tags" column from relevant metadata  
   - Convert text into vectors using `CountVectorizer`  
4. **Similarity Model**:  
   - Compute cosine similarity between movie vectors  
   - Recommend top N similar movies for any given title  

---

## How to Use  
1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
