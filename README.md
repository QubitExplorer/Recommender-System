# Recommender Systems: Let me tell you a story!

#Writing in progress

Instead of throwing around random mathematical derivations for Recommendation Engine or recommender systems, I finally decided to write stories. When I started writing this page, I knew nothing about recommendation engine.  So, let's take a guess: what are they, how it might work, why do we need them in our daily lives and how we can leverage it further ?

To understand this, lets imagine we are in the year 1750's. You're in your mid-twenties, it's been your childhood dream to buy a **new horse**, since there's no Ferrari and Tesla at the time. You have dreamed about it several days, weeks and even months, and finally after saving few coins everyday, you have saved enough. Now, have enough big coins to buy a new horse. But you **do not know which one to buy** and **where to buy it**. So, what would you do now ?. Well, you did probably ask for a **recommendations or suggestions** from people with experience **(i.e. past data)**, and **who shares similar interest** and you like to gather advise from each one of them. 

----------------------------------------------------------------------------------------------------------------
Lets say, You have three best friends, and all of them were having equal knowledge but totally different varities of interests:

As a User (Horse Buyer), you personaly like: **Football, Hiking, Climbing, Animal Caretaking and Reading**

Friend A: Enjoys **Football, Hiking, Running, Animal Caretaker and Climbing**

Friend B: Prefer Singing, Writing and Reading.

Friend C: Likes Bicycling (It seems that there is no bicycles until 1817, anyway its a story) and Singing.  

----------------------------------------------------------------------------------------------------------------

Clearly,  **Friend A** has similar interest more similar to you and you would **assign more weightage ** to him, right ?. In neural networks it called "weights". 

Now, its just about three friends with eight different interest, which is easier for calculations. What would be the case if you have (100 million) 100, 000, 000 friends and all of them were having 50,000 different varities of interesting data points. Well, we may need to invite math experts to perform this set of calculations, or else we need an advanced computers to perform this huge operations. Luckily, the invention of Transitors in 1940's provided the path to highly advanced office tools called "MS Excel" by which you can perform approx 1 million data points i.e 10, 48,576 rows to be precious, just press ctrl + down, you will reach there (Technically, csv file can handle more than that, but still it has limitations for modern recommendater systems). Basically we can use some build in data analysis statistical functions like correlations, and cosine similarities to calculate and to identify similar users (below is the example).

![image](https://github.com/user-attachments/assets/4a8e2dd7-ef3e-4eeb-823e-9b0111a6f95f)


In big data, excel cannot handle such billion's of data volumn, so we can calculate the **cosine similarities** between one user with respect to other 100 Million friendly users who agreed to share their music watch history and will get a combinations of roughly 1 quatrillion cosine score values which you can store it in on-prem server (and in recent years all most all fortune 500 companies migrated it to cloud).  You can slice and dice the data (ETL) in cloud, apply different statistical concepts, whatever makes sense to you, get the best, quick yet practical results. This is how companies like Netflix and Amazon recommends thousands of products daily. 

The field of AI and ML is still young - 15 years old - keeps evolving.  Somewhere along the way, the concept known as "Recommendation Engine". Millions of data scientists use this nomenclature nowadays. Maybe the techniques might be different, yet the core concept is still the same. Then comes the time series problem: yesterday you bought a horse, today you might buy a cute dog and what would you buy tomorrow ?. It's the basic time series tasks. 

 1. Amazon - Started in a garage once, to suggest similar products which we likely to hit enter and buy it, today its market value around 1.97 trillion us dollers,
 2. Netflix (~322 billion USD) - where we indulge into our favorite movies without even glancing at the clock, and
 3. Spotify (~ 74 Billion USD) - Where we listen similar songs and music which we preferably fell in love with, is all about recommendion engines. 

We could also calculate **correlations** and get the similar products which is similar to horse and can suggest other users as well. 

Here, we will be further exploring different varieties of recommendation algorithms available today and we also going to develop new customizable model using deep learning techniques like RNN, CNN, and LSTM, over several iterations. Similarly, In modern days there are varieties of recommender systems available and below are the two major types:
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
14. Other Hybrid Approcahes.

Here, we will be leveraging RecBole libraries to explore various models and to develop more customizable one. Ref: https://recbole.io/

List of Different Varieties of Datasets:

![image](https://github.com/user-attachments/assets/e842adf0-6eaa-48b7-9ffa-68312db0788e)

Comparision and Performance Results For All Approaches:

Yet to be added.
