# Article-summary-using-deeplearning
PROJECT
ARTICLE SUMMARY DEEP LEARNING
SUMMARY
Using deep learning and scraping to analyze/summarize articles! Just drop in any URL!
![intro](https://ianramzy.com/res/projects/article-summary-deep-learning/article-summary-deep-learning1.png)


    
INSTALLATION & USAGE
Github Repo
# You will need to have Python 3 and Pip installed

$ git clone https://github.com/saran-gangster/Article-summary-using-deeplearning.git

$ cd article-summary-deep-learning

$ pip install -r requirements.txt

$ python -m spacy download en_core_web_sm

$ python app.py

INSPIRATION
In a day and age where information is not only abundant but overflowing, I wanted to create a faster way parse all of it. I originally wanted a browser extension that would summarize any page that I was reading in a few bullet points so that I could save time. But I later settled on a web app for more flexibility.

WHAT IT DOES
The application takes in a URL and makes request to that page scraping all of the data from it. The data is then cleaned (removing noise) and a name entity recognition is performed where all entities are labeled in the text (that's the cool visualization/highlighted part). It then takes the most common entity in the text and assumes it is the subject of the article and proceeds to extract facts from the text itself and renders the frontend.

TECHNOLOGIES
The web application is built using flask, and the frontend is pure css and html. For web scraping beautifulsoup4 was used and deep learning was done using Spacy and textacy. Specifically Spacy for named entity recognition (NER) and textacy for sentence structure analysis.

FUTURE IDEAS AND WHATS NEXT
I would like to gather more data for training the models. And I would also like to add a feature where the algorithm will look for more sources on the internet about a topic (i.e. Obama) and gather more data to analyse there.

Another project by B2l Industries
