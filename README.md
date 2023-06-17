# LeetCompass
An web application to surf Leetcode question(will integrate other coding platforms later)


# Search Engine

This is a simple search engine implemented using Flask framework in Python. The search engine allows users to enter a search term and retrieve relevant documents based on TF-IDF (Term Frequency-Inverse Document Frequency) ranking.

## Web Application

It uses [TF-IDF](https://en.wikipedia.org/wiki/Tf%E2%80%93idf) Algorithm to implement search. The server is live on https://leetcompasss.onrender.com/.

## Requirements

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

![Flask](https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white)

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)

![Bootstrap](https://img.shields.io/badge/bootstrap-%238511FA.svg?style=for-the-badge&logo=bootstrap&logoColor=white)

![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)


## Installation

1. Clone the repository :
   ```bash
   git clone https://github.com/Tiyas17/LeetCompass.git
   cd LeetCompass
   ```
2. Install the required dependencies using pip :
   ```bash
   pip install flask
   pip install flask-wtf
   pip install chardet
   ```
3. Delete tf-idf folder 

4. Run the `prepare.py` script to make tf-idf folder :
   ```bash
   python -u prepare.py
   ```
5. Run `app.py` to check the working of server


## Running the Search Engine

To start the search engine, run the following command:

```bash
flask --app app run
```

Open your web browser and visit `http://127.0.0.1:5000` to access the search engine user interface.

## Search Functionality

The search engine offers an uncomplicated interface that allows users to input a search term and indicate the desired number of questions to retrieve. After submitting the search query, the search engine evaluates the TF-IDF score for each document and presents the most relevant documents based on the query. The search functionality is executed through the calculate_sorted_order_of_documents() function, which accepts a list of query terms and generates a sorted list of documents along with their scores and question links.

## User Interface

The user interface is implemented using HTML templates and Bootstrap CSS framework. The main interface consists of a search form where users can enter their search term and select the number of questions to retrieve. The search results are displayed as cards, showing the document text and a link to the corresponding question.
For Demo : visit `[https://leetcompasss.onrender.com]`

## Conclusion

This search engine provides a basic implementation of a TF-IDF ranking-based search algorithm. It can be further enhanced with additional features such as relevance feedback, query expansion, and more sophisticated ranking algorithms. Feel free to explore and customize the code according to your requirements.

