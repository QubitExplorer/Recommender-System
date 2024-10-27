# Recommendation-Engine: Let me write in my own words!

#Writing in progress

While, I do not know anything about recommendation engine when I started writing this page, but let's guess what it could be, how it might work, why we need this recommendation engine in our day to day life and how we can leverage it further. 

Maybe, Let's go back to the golden year 1750's. Let's assume you are in your mid-twenties and it's your childhood dream to buy a **new horse**, since we don't have Ferrari, BMW at that time. You kept dreamt about it several days, weeks and finally started saving penny amount of coins everyday over the period of last several months. Finally you reached your target, made it, and have enough big coins to buy a new horse, but you **do not know which one to buy** and **where to buy it**. So, now what would we do ?. Well, Lets ask for a **recommendations or suggestions** from the one who have experience **(i.e. past data)**, whom you trust the most **(like-minded or who shares similar interest)** and will note down a list of recommendations. 


----------------------------------------------------------------------------------------------------------------
You have three best friends, and all of them are having a equal knowledge but different interests:

As a User (Horse Buyer), you personaly like: **Football, Hiking, Climbing and Reading**

Friend A: He likes **Football, Hiking, Running, Climbing and Reading**

Friend B: Likes Singing, Writing and reading books.

Friend C: Likes Cycling (assuming there would be some bicycles on those days) and Singing.  

----------------------------------------------------------------------------------------------------------------

Obviously, here **Friend A** has a similar interest like you and you would **assign more weightage** to him, right ?.

Now, its just the case of 3 friends with 8 different interest. What would be the case if you have 100, 000, 000 (100 million) friends and all of them were having 50,000 different varities of interesting data points. Well, we may need to invite "Ramanujan" (The Man who Infinity) to perform this set of operations, or we need a super computers to perform huge operations. Basically we can calculate the **cosine similarities** between one user with respect to other 100 Million friendly users who agreed to share their music history data and will get a combinations of roughly 1 quatrillion cosine scores values.  You can slice and dice the data (ETL), apply different statistical concepts, whatever it makes sense to you, gets the best and quick results. This is how the big companies like Netflix, Amazon perform mathematical operations and recommends thousands of the similar products in our day to day. 

Almost, Every one is pretty new in this AI/ML era, its just 10 years old, it keep evolving over the period of time. Maybe some one has named it as "Recommender Engine" couple of years before and thats how the millions of data and computers scientists were following the similar nomenclature in recent years. Just the techniques might be different, but the concept is same. 

 1. Amazon (Market Cap: 1.97 Trillion USD) - Started in a garage once, to suggest similar products which we likely to hit enter and buy it,
 2. Netflix (~322 billion USD) - where we indulge into our favorite movies without even glancing at the clock, and
 3. Spotify (~ 74 Billion USD) - Where we listen similar songs and music which we preferably fell in love with, is all about recommendion engines. 

We could also calculate **correlations** and get the similar products which is similar to horse and can suggest other users as well. 

Here, we will be further exploring different varieties of recommendation algorithms available today and we also going to develop new customizable model using deep learning techniques like RNN, CNN, and LSTM, over several iterations. Similary, In modern days there are varieties of recommendation systems available and below are the two major types:
1. Collaborative Filtering (User to User), and
2. Content Based Filtering (Product to Product).

Different Methods to identify User similarities:
1. Correlations,
2. Cosine Similarities,
3. Jaccard Similarities,
4. Euclidean Distance,
5. Hamming Distance, 
6. Manhatten Distance,
7. Bhattachryya Distance,
8. Neural Network Embeddings (Collaborative Filtering), and
9. Kullback Leibler divergence,
10. Embeddings and Latent Features,
11. Sequence-Based Similarity,
12. Deep Collaborative Filtering with Embeddings (via Neural Networks),
13. Transformer Models for Sequential Recommendations (e.g., BERT4Rec), and 
14. Other Hybrid Approcahes. 

Here, we will be leveraging RecBole libraries to explore various models and to develop more customizable one. Ref: https://recbole.io/

List of Different Varieties of Datasets:

![image](https://github.com/user-attachments/assets/e842adf0-6eaa-48b7-9ffa-68312db0788e)

Comparision or Performance Results For All Approaches:

Yet to be added.
