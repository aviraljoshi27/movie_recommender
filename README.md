# Movie Recommender
Recommender system can be of 3 types:
1. Content  based : It'll recommend according the past content consumption.
2. Collaborative based : If there  are two user who are very similar, so if one like something we can recommend it to other one also.
3. Hybrid based : Combination of both.

In this project we are using CONTENT based recommender system.

Step 1: We will start with data: (Pre processing)
Step 2 : Create a ML model.
Step 3: Create a website.
Step 4: Deploy it.

VECTORIZATION: We have three columns name, id, tags
    --> we have to vectorize the tags.
    --> it'll make each  movie a vector.
    --> then the closest vectors will be similar movies.
    --> we use bag of words to vectorize

BAG OF WORDS:
    --> we will combine all the words
    --> we will take out the words with most frequency (5000 words)
    --> we will check these extracted word in tags of each movie.
    --> now the shape is 5000 movies * 5000 words, basically it became 5000D vector.
    --> in this we will not consider stop words(e.g. is, are, to, be etc.)
    --> we will use scikit library.
    --> the we stem these word (i.e. to covert them to root word) using nltk library.
    --> then we calculate the COSINE distance not euclidean distance between these vectors.
    
    