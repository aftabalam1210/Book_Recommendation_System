

# 📚 Book Recommendation System

This is a simple Book Recommendation System built using **Flask**, **Scikit-learn**, and **Pickle** for serving precomputed recommendation results. It allows users to get personalized book recommendations based on a selected book.

## 🚀 Features

* View the most popular books with ratings and vote counts.
* Get book recommendations based on a selected title.
* Simple and clean web interface built with HTML and Flask.

## 🧰 Tech Stack

* Python
* Flask
* Numpy, Pandas
* Scikit-learn (for similarity matrix)
* Pickle (for serialized data)
* HTML/CSS (for frontend)

## 📁 Project Structure

```
.
├── app.py                      # Main Flask application
├── book.ipynb                  # Jupyter notebook for data preprocessing
├── Books.csv                   # Raw book metadata
├── Ratings.csv                 # Raw ratings data
├── Users.csv                   # Raw user data
├── books.pkl                   # Serialized books DataFrame
├── popular.pkl                 # Popular books (title, author, rating, image)
├── pt.pkl                      # Pivot table (user-item matrix)
├── similarity_scores.pkl       # Precomputed cosine similarity scores
├── templates/
│   ├── index.html              # Homepage template
│   └── recommend.html          # Recommendation UI

```

## 🔧 Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/book-recommendation-system.git
cd book-recommendation-system
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Make sure the following pickle files are present

* `popular.pkl`
* `pt.pkl`
* `books.pkl`
* `similarity_scores.pkl`

> These files contain the processed data and must be present in the root directory.

### 4. Run the application

```bash
python app.py
```

The app will be running at `http://127.0.0.1:5000/`.

## 📸 Screenshots
*HomePage*
![image](https://github.com/user-attachments/assets/6913de0b-51a6-4069-9e6f-5d5bcfbf3249)

*Recommendation Page*
![image](https://github.com/user-attachments/assets/dcecdb91-66f6-4ac9-9be0-e2f80911f337)


### Homepage

Displays the most popular books with average ratings.

### Recommendation Page

Input a book name and receive similar book recommendations.

## 📌 Notes

* This project uses a simple item-based collaborative filtering method.
* You must preprocess the dataset and generate `.pkl` files before running the app.

## 🙌 Acknowledgements

* [Book-Crossing Dataset](http://www2.informatik.uni-freiburg.de/~cziegler/BX/)
* Inspiration from various tutorials and community projects

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.


