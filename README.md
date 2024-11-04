# Recommender Systems: Let me tell you a story!


Instead of throwing around random mathematical derivations for recommendation engine or recommender systems, I finally decided to write story. When I started writing this page, I knew nothing about recommendation engine.  So, let's take a guess: what are they, how it might work, why do we need them in our daily lives and how we can leverage it for various real life use cases.

To understand this, lets imagine we are in the year 1750's. You're in your mid-twenties, it's been your dream to buy a **new horse**, since there's no Ferrari and Tesla at the time. You have dreamed about it several days, weeks and even months, and finally after saving few coins everyday, you have saved enough. Now, you have enough big coins to buy a new horse. But you **do not know which one to buy** and **where to buy it**. So, what would you do now ?. Well, you did probably ask for a **recommendations or suggestions** from people with experience **(i.e. past data)**, and **who shares similar interest** and you like to gather advise from each one of them. 

----------------------------------------------------------------------------------------------------------------
Lets say, You have three best friends, and all of them were having equal knowledge but totally different varities of interests:

As a User (Horse Buyer), you personaly like: **Football, Hiking, Climbing, Animal Caretaking and Reading**

Friend A: Enjoys **Football, Hiking, Running, Animal Caretaker and Climbing**

Friend B: Prefer Singing, Writing and Reading.

Friend C: Likes Bicycling (It seems that there is no bicycles until 1817, anyway its a story) and Singing.  

----------------------------------------------------------------------------------------------------------------

Clearly,  **Friend A** has similar interest more similar to you and you would **assign more weightage ** to him/her, right ?. In neural networks it called "weights". 

Now, its just about three friends with eight different interest, which is easier for calculations. What would be the case if we have (100 million) 100, 000, 000 friends and all of them were having 50,000 different varities of interesting data points. Well, we may need to invite math experts to perform this set of calculations, or else we need an advanced computers to perform this huge operations. 

Luckily, the invention of Transitors in 1940's provided the path to highly advanced office tools called "MS Excel" by which we can perform approx 1 million data points i.e 10, 48,576 rows to be precious, just press ctrl + down, you will reach there (Technically, csv file can handle more than that, but still it has limitations for modern recommender systems). 

Basically we can use some build in data analysis statistical functions like correlations, and cosine similarities to calculate and to identify similar users (below is the basic example).

![image](https://github.com/user-attachments/assets/a102eda4-475a-42f1-a692-e90480215c5e)

![image](https://github.com/user-attachments/assets/937a996b-487a-436b-8329-4b950d9cfad1)

It's a very basic example and there are some drawbacks associated with it, like sparse (zero) values, curse of dimensionality etc.,

In big data world, excel cannot handle such billion's of data volumn, so we can calculate the **cosine similarities** between one user with respect to other 100 Million friendly users who agreed to share their music watch history and we will get a combinations of roughly 1 quatrillion cosine score values which you can store it in on-prem database server (and in recent years all most all major companies migrated it to cloud/hybrid models).  We can slice and dice the data (ETL - Extract Transform and Load) in cloud, apply different statistical concepts, whatever makes sense to us, get the best, quick yet practical results. This is how companies like Netflix and Amazon recommends thousands of products daily. 

The field of AI and ML is still young - maybe 20 years old - keeps evolving.  Somewhere along the way, the concept became as "Recommender Systems". Millions of data scientists use this nomenclature nowadays. Maybe the recent techniques might be different, yet the core concept and unique benefit (value proposition) is still the same, **recommend the best product/service to the user**. Then comes the time series problem: yesterday we bought a horse, today we might buy a cute dog and how about tomorrow ?. It's the basic time series tasks. 

Here are the few examples of companies using recommendation engines:
 1. Amazon - To suggest similar products which we likely to hit enter and buy it, today its market value around 1.97 trillion us dollers,
 2. Netflix - We indulge into our favorite movies without even glancing at the clock, valued around 322 billion USD, and
 3. Spotify - Where we listen similar songs and music which we preferably like it, valued appox 74 billion USD.
 4. Google Maps - Helps us to reach our favorite destination on time, without rushing. This is important for our below use cases.

Here, we will be further exploring different varieties of recommendation algorithms available today and we also going to develop new customizable model using deep learning techniques like RNN, CNN, and LSTM. Similarly, In modern days there are varieties of recommender systems available and below are the two major types:
1. Collaborative Filtering (User to User), and
2. Content Based Filtering (Product to Product).

Different Methods to identify User similarities:
1. Correlations,
2. Cosine Similarities,
3. Jaccard Similarities,
4. Euclidean Distance, (measuring straight line distances, even distance between Vienna to Dublin or Dublin to Chennai. In 3 dimensions!)
5. Hamming Distance, 
6. Manhatten Distance,
7. Bhattachryya Distance,
8. Neural Network Embeddings (Collaborative Filtering),
9. Kullback Leibler divergence,
10. Embeddings and Latent Features,
11. Sequence-Based Similarity,
12. Deep Collaborative Filtering with Embeddings (via Neural Networks),
13. Transformer Models for Sequential Recommendations (e.g., BERT4Rec), and
14. In life science application (some techniques used for DNA Sequencing to find the similarities, which clould also be leveraged for RC)
15. Other Hybrid Approches.

Here, we will be leveraging RecBole libraries to explore various models and to develop more customizable one. Ref: https://recbole.io/

List of Different Varieties of Datasets:

![image](https://github.com/user-attachments/assets/e842adf0-6eaa-48b7-9ffa-68312db0788e)

Comparision and Performance Results For All Approaches:
1st set of results for the simple BPR model with 10 epochs, for movielens datasets: (To be fine tuned further)

![image](https://github.com/user-attachments/assets/d2bf1736-6617-4afc-9dbe-88134e8e40fe)

Functions like a Minimum Viable Product (MVP):

![image](https://github.com/user-attachments/assets/d157ae60-54c2-41e8-9bf3-e79e1250bc1b)

**Agile Method:** Or, we can also do in an Agile Way - Summary for the Compiler Process:

Lexical Analysis: Backlog is broken down into workable tasks.  

Syntax Analysis: Ensures tasks fit the plan.

Semantic Analysis: Verifies that the output delivers meaningful value. 

Optimization: Continuous improvement and refinement of the product. 

Code Generation: Delivers a working increment of software. 


**Recbole - Major Classifications:**

General Recommendation (GR): The interaction of users and items is the only data that can be used by model. Usually, the models are trained on implicit feedback data and evaluated under the task of top-n recommendation. All the collaborative filter (CF) based models are classified in this class.

Content-aware Recommendation: This can be seen as an extension of click-through rate prediction. All the model in this class can be used for CTR prediction. Usually, the dataset is explicit and contains label field. Other feature fields are also support for these models. And evaluation is always conducted in the way of binary classification.

Sequential Recommendation: Similar to time series problem, which we discussed earlier. The task of SR (next-item recommendation) is the same as GR which sorts a list of items according to preference. While the history interactions are organized in sequences and the model tends to characterize the sequential data. The models of session-based recommendation are also included in this category.

Knowledge-based Recommendation: Knowledge-based recommendation introduces an external knowledge graph to enhance general or sequential recommendation.

Evaluation Metrics: Recall, Precision, ndcg. 

References:
1. https://recbole.io/docs/user_guide/model/general/bpr.html
2. https://recbole.io/
3. https://grouplens.org/datasets/movielens/100k/
