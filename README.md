# 🎬 Movie Recommender System

An interactive **Movie Recommendation System** built with **Streamlit** that suggests similar movies based on user input.  
The app integrates with the **TMDB API** to fetch movie posters, trailers, and details, providing an engaging movie discovery experience.  

---

## 🚀 Features
- 🎥 **Movie Recommendations** — Get 5 similar movies for any selected title.  
- 🖼️ **Dynamic Posters** — Fetches high-quality posters from TMDB.  
- ▶️ **Trailers** — Click poster thumbnails to watch trailers directly on YouTube.  
- 🔗 **Movie Links** — Quick access to official TMDB movie pages.  
- 🎨 **Custom UI** — Netflix-themed background, hover effects, and styled components.  

---

## 📂 Project Structure
.
├── app.py # Main Streamlit application
├── movie_list.pkl # Pickled movie metadata (titles + IDs)
├── similarity.pkl # Pickled similarity matrix
├── netflix.jpg # Background image
└── README.md # Project documentation

yaml
Copy
Edit

---

## 🛠️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/movie-recommender.git
cd movie-recommender
```
2. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
Requirements include:

streamlit

requests

pickle

pandas

scikit-learn (for similarity matrix creation)

3. Data Files
Ensure the following files are present:

movie_list.pkl — contains movie metadata (title, TMDB ID, etc.)

similarity.pkl — precomputed similarity scores between movies

(You can generate these from your dataset or use the pre-trained files if provided.)

4. Run the App
bash
Copy
Edit
streamlit run app.py
🌐 API Integration
This app uses the TMDB API for movie posters and trailers.
You need a TMDB API key to run it:

Create an account at TMDB.

Go to Settings > API and generate an API key.

Replace the API key inside app.py:

python
Copy
Edit
api_key = "YOUR_TMDB_API_KEY"
🎨 UI Preview
The app has a Netflix-inspired theme with:

Full-page background (netflix.jpg)

Hover animations on posters

Styled headers and buttons

(Add screenshots here for better presentation)

markdown
Copy
Edit
![App Screenshot](Images/screenshot1.png)
![App Screenshot](Images/screenshot2.png)
✨ Future Improvements
Add user ratings & collaborative filtering.

Support for TV Shows as well as movies.

Deploy on Streamlit Cloud / Heroku / Vercel for live demo.

📌 Example
Search for Inception → instantly get recommended movies like Interstellar, The Dark Knight, etc. with posters, trailers, and links.
