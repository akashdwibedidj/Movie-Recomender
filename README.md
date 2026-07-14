# Movie Recommender System

A content-based movie recommendation system that suggests similar movies based on a selected title. Built using Python, pandas, and scikit-learn, with a similarity matrix computed from movie metadata (genres, cast, crew, keywords, and overview).

## 🔗 Repository

[https://github.com/akashdwibedidj/Movie-Recomender](https://github.com/akashdwibedidj/Movie-Recomender)

## 📌 Features

- Recommends top similar movies based on content similarity
- Uses vectorization (e.g., CountVectorizer / TF-IDF) on combined movie tags
- Cosine similarity used to compute closeness between movies
- Precomputed similarity matrix for fast lookups

## 🗂️ Project Structure

```
Movie-Recomender/
├── movie_recomender_system.ipynb   # Main notebook: data processing, feature engineering, model building
├── setup.sh                        # Setup script for environment/dependencies
├── requirements.txt                # Python dependencies
├── .gitignore
└── README.md
```

> Note: Generated artifacts like `movies.pkl`, `movie_dict.pkl`, and `similarity.pkl` are created by running the notebook and are not tracked in this repo (see `.gitignore`).

## ⚙️ Setup & Installation

1. Clone the repository
   ```bash
   git clone https://github.com/akashdwibedidj/Movie-Recomender.git
   cd Movie-Recomender
   ```

2. Create and activate a virtual environment
   ```bash
   python -m venv .venv
   .venv\Scripts\activate      # Windows
   source .venv/bin/activate   # macOS/Linux
   ```

3. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

4. Run the setup script (if applicable)
   ```bash
   bash setup.sh
   ```

5. Launch the notebook
   ```bash
   jupyter notebook movie_recomender_system.ipynb
   ```

## 🚀 Usage

Run all cells in `movie_recomender_system.ipynb` to:
1. Load and preprocess the movie dataset
2. Engineer features (tags from genres, cast, crew, keywords, overview)
3. Vectorize text data and compute cosine similarity
4. Generate `movies.pkl`, `movie_dict.pkl`, and `similarity.pkl` for use in a recommendation app

Once the pickle files are generated, you can use them to build a front-end (e.g., Streamlit app) to search for a movie and get recommendations.

## 📊 Dataset

This project uses a movie metadata dataset (e.g., TMDB 5000 Movie Dataset) containing information such as titles, genres, cast, crew, keywords, and overviews.

## 🛠️ Tech Stack

- Python
- pandas, numpy
- scikit-learn
- Jupyter Notebook

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome. Feel free to open a pull request or issue.