# Recommender-System: Let me write in my own words!

In simple terms, We us human tend to perceive things around us and often tend to recommend any new products, services to our loved one, they can our friends, family and even our collegues, whenever we like something the most. Similarly in big data world, recommender systems is anything that suggests similar products, services to certain audience who share the common interest. For example., The most powerful recommendation engine which is available today is, 1. Amazon - to suggest similar products which we likely to hit enter and close the deal, 2. Netflix - where we spend lot of time without even checking the clock, 3. Spotify to suggest similar songs and music which we preferably fell in love with, is all recommender engines around us. 

Here, we will be exploring various types of recommendation algorithms available today and we also going to develop new customizable model using deep learning techniques like RNN, CNN, and LSTM, over several iterations.

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

