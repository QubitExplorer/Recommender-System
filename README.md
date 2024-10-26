# Recommender-System: Let me write in my own words!

#Work in progress

Well, I do not know anything about recommendation engine while I started writing this page, but let's guess what it could be, how it might work, why we need this recommendation engine in our day to daya life and how we can leverage it further. 

Maybe, Let's go back to the golden year 1750's. Lets assume you are in your mid-twenties and it's your childhood dream to buy a **new horse**, since we don't have Ferrari, BMW at that time. You kept dreamt about it several days, weeks and finally started saving penny amount of coins everyday over the period of last several months. Finally you made it, and have enough big coins to buy a new horse, but you **do not know which one to buy** and **where to buy it**. So, now what would we do ?. Well, Lets ask for a **recommendations or suggestions** from the one who have experience **(i.e. past data)**, whom you trust **(like minded or who shares similar interest)** and will collect a list of recommendations. 

You have three best friends, and all of them are having a equal knowledge but different interests:

As a User (Horse Buyer), you personaly like: **Football, Hiking, Climbing and Reading**

Friend A: He likes **Football, Hiking, Running, Climbing and Reading**

Friend B: Likes Singing, Writing and reading books.

Friend C: Likes Cycling (assuming there would be some bicycles on those days) and Singing.  

Obviously, here Friend A has a similar interest like you and you would assign more weightage to him, right ?.

Now, its the case of 3 friends with 8 different interest. What's would be the case if you have 100, 000, 0000 million friends and all of them were having 1000, 000, 0000 different varities of interesting data points. Well, we may need to call "Ramanujan" (The Man who Infinity), or we need a super computer to perform huge operations.  

Every one is pretty new, and some one has named it as "Recommender Engine" and the rest of millions of data & computers scientists might have read and started following the similar naming nomenclature in recent years. Just the techniques were different, but the basic concept is same. 
The one is who is first and developed the best algorithm were:

 1. Amazon (~ Valued today around 1.97 Trillion USD) - Started in a garage - to suggest similar products which we likely to hit enter and close the deal
 2. Netflix (~322 billion USD) - where we spend lot of time without even checking the clock and
 3. Spotify (~ 74 Billion USD) - to suggest similar songs and musics which we preferably fell in love with, is all recommender engines do around us. 

We have a super computers to perform such operations, 

Basically we can calculate the **cosine similarities** between one user with respect to other 1 Million friendly users who agreed to share their usage data adhering to GDPR and other data regulations and we are allowed to calculate and will get a combinations of roughly xxxx cosine scores.  This is how Netflix, Amazon perform operations and recommends us the similar products in the ecommerce websites. 

You could also calculate **correlations** and get the similar products which is similar to horse and can suggest other users as well. 

Here, we will be further exploring different varieties of recommendation algorithms available today and we also going to develop new customizable model using deep learning techniques like RNN, CNN, and LSTM, over several iterations.

Similary, In modern days there are varieties of recommendation systems available and below are the two primary types:
1. Collaborative Filtering (User to User), and
2. Content Based Filtering (Product to Product).

Here, we will be leveraging RecBole libraries to explore various models and to develop more customizable one. I hope this make sense to some extent. 

Ref: https://recbole.io/

List of Different Varieties of Datasets:

![image](https://github.com/user-attachments/assets/e842adf0-6eaa-48b7-9ffa-68312db0788e)

