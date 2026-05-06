# 🎬 Movie Recommender System
## 📄 Description
A personalized **movie recommendation** web application that suggests films based on content similarity. 
Users can interact with a visual interface, select movies they enjoy, and receive tailored suggestions in real-time.

---

## 🔗 Live Deployment 
#### Paste this in your browser:
```
recommender-app-1.onrender.com
```

## ✨ Features
- **Interactive UI**: A grid-based selection system allowing users to pick movies they like.
- **Content-Based Filtering** :Recommends movies by analyzing metadata (genres, descriptions, etc.) from the Cleaned_Movies.csv dataset.
- **Similarity Matrix**: Utilizes a pre-computed similarity.pkl matrix (Cosine Similarity) for lightning-fast recommendations.
- **Responsive Design** : Seamlessly deployed on Render for global access.  

---

## 🛠️ Technical Stack

- **Backend** : Flask (Python)
- **Data Processing** : Pandas, NumPy
- **Machine Learning** : Scikit-learn (TF-IDF Vectorization, Cosine Similarity)
- **Serialization** : Pickle
- **Frontend** : HTML5, CSS3, JavaScript (Fetch API)
- **Deployment**: Render

---

## 🧠 Working Principle

The app uses Content-Based Filtering. Every movie is converted into a multi-dimensional vector based on its features. 
When a user selects a movie, the system calculates the "distance" between that movie and all others in the database using Cosine Similarity.

- **TF-IDF Vectorization** : Textual data is converted into numerical vectors.
- **Cosine Similarity** : The app calculates the cosine of the angle between vectors. A smaller angle (value closer to 1) indicates higher similarity.
- **Recommendation Engine** : The top N movies with the highest similarity scores to the user's selection are returned.

---

## 📥 Installation & Local Setup
If you want to run this project locally, follow these steps:
#### Clone the repository:
```bash
git clone https://github.com/Bruhrk42/recommender_app.git
cd recommender_app
```
#### Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
#### Install dependencies:
```bash
pip install flask pandas scikit-learn
```
#### Ensure Data Files are present:
Make sure Cleaned_Movies.csv and similarity.pkl are in the root directory.

####
```bash
python recommender.py
```

Open http://127.0.0.1:5000 in your browser.

---

## 📊 Dataset
#### The system uses a dataset containing:
- Movie Titles
- Genres
- Plot Overviews
- Poster Images (stored in the /images folder)

## 🤝 Contributing
#### Contributions are welcome! If you have suggestions for improving the recommendation algorithm or the UI, please fork the repo and create a pull request.
Fork the Project \
\
Create your Feature Branch 
```bash
git checkout -b feature/AmazingFeature
```
Commit your Changes 
```bash
git commit -m 'Add some AmazingFeature'
```

Push to the Branch 
```bash
git push origin feature/AmazingFeature
```

Open a Pull Request

---

## 📝 License

#### Distributed under the MIT License. See LICENSE for more information.
**Author**: Bruhrk42
