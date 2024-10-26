# Recommender-System: Let me write in my own words!

#Work in progress

Well, I do not know anything about recommendation engine while I started writing this page, but let's guess what it could be, how it might work, why we need this recommendation engine in our day to daya life and how we can leverage it further. 

Maybe, Let's go back to the golden year 1750's. Lets assume you are in your mid-twenties and it's your childhood dream to buy a **new horse**, since we don't have Ferrari, BMW at that time. You kept dreamt about it several days, weeks and finally started saving penny amount of coins everyday over the period of last several months. Finally you made it, and have enough big coins to buy a new horse, but you **do not know which one to buy** and **where to buy it**. So, now what would we do ?. Well, Lets ask for a **recommendations or suggestions** from the one who have experience **(i.e. past data)**, whom you trust **(like minded or who shares similar interest)** and will collect a list of recommendations. 

You have three best friends, and all of them are having a equal knowledge but different interests:

As a User (Horse Buyer), I personaly like: **Football, Hiking, Climbing and Reading**

Friend A: He likes **Football, Hiking, Running, Climbing and Reading**

Friend B: Likes Singing, Writing and reading books.

Friend C: Likes Cycling (assuming there would be some bicycles on those days) and Singing.  

Obviously, Friend A has a similar interest like me and I would assign more weightage to him. 


In simple terms, We us human tend to perceive things around us and often tend to recommend any new products, services to our loved one, they can our friends, family and even our collegues, whenever we like something the most. Similarly in big data world, recommender systems is anything that suggests similar products, services to certain audience who share the common interest. For example., The most powerful recommendation engine which is available today is, 1. Amazon - to suggest similar products which we likely to hit enter and close the deal, 2. Netflix - where we spend lot of time without even checking the clock, 3. Spotify to suggest similar songs and music which we preferably fell in love with, is all recommender engines around us. 

Here, we will be exploring various types of recommendation algorithms available today and we also going to develop new customizable model using deep learning techniques like RNN, CNN, and LSTM, over several iterations.


**Restaurant Example:**
Lets, start with the basic question, how and with whom would you recommend ?. To answer this, lets go restaraunt and I'm feeling like hungry now. Now, I would try some new food which I haven't done it before and at the same time I don't want to spend money and waste my time to try something which I may not like. Now, what we do is ask for a **recommendations or suggestions** from a friend or waiter over there. Lets assume, we got few suggestions from our friends to try for Food A, Food B and Food C. Which would one you pick and how would choose the food ?. In case, if we live in 1650's, where we don't have electronic gadgets, our human brain would subconsiously analyze the situation quickly and would propose "yes" or "No" situation. Either we would trust our friend or a waiter, but we do not know who is the best like minded folk. 

To do that, 

Friend - Past Data, we know him, his likes, dislikes. If we have a high correlation or cosine similarity, then we would like likely to "Yes". Other "No".

Waiter (in the restaurant) - In this case, Its like a new user data, where you try it out and see, little risk for the first time. 

Similary, In modern days there are varieties of recommendation systems available and below are the two primary types:
1. Collaborative Filtering (User to User), and
2. Content Based Filtering (Product to Product).

Here, we will be leveraging RecBole libraries to explore various models and to develop more customizable one.

Ref: https://recbole.io/

List of Different Varieties of Datasets:

![image](https://github.com/user-attachments/assets/e842adf0-6eaa-48b7-9ffa-68312db0788e)

