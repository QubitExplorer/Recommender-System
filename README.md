# Recommender Systems: Let me tell you a story!

Audio Podcast Version: https://notebooklm.google.com/notebook/4bdd617f-a731-45eb-b3e6-3cdc2d7479d2/audio

At its core, a **recommendation engine** uses computer algorithms to predict and suggest items of interest to users based on their past behaviors and contextual data. On the deep learning front, xLSTM (extended LSTM) and Transformers have been evolved with latest architectures in recent years and plays a very important role in Large Language Models. 

Since recommenders have became an essential part of our daily digital experiences, in this paper we will be leveraging XLSTM architecture based recommenders and will be comparing the results with other modern architectures like Autotransformers, Recurring Neural Networks (RNN) and other Matrix Factorization Methods. xLSTM incorporates architectural enhancements like attention mechanism, gating improvments and bidirectional capabilities. It will be impactful due to several unique aspects when to compared to the tradional successful methods. 

**Existing Approaches:**
**Transformers Based:** Uses the self-attention mechanism from transformer architectures (like in GPT or BERT) to model the user-item interactions. It also captures the complex sequential patterns in user behavior (e.g., purchase history or clicks) and finally makes personalized recommendations by understanding the contextual relationships between items and users. Unlike, RNN which process information sequencially (one step at a time), transformer process information in parallel utilizing the self attentio mechanism which results in faster computation precerving long term dependencies.

A transformer-based recommender system uses an embedding layer to convert the users and items into dense vector representations. It applies self-attention layers to capture complex dependencies and sequential relationships in user-item interactions, enhanced by positional encodings to preserve and keep the order of actions. The final output layer computes scores or rankings to predict the most relevant items for each user.

**Matrix Factorization Based:** It decompose a user-item interaction matrix into two smaller matrices: one representing users and the other representing items. These matrices capture latent factors (hidden patterns) that explain the user preferences and item characteristics. By reconstructing the original matrix, the system predicts how much a user might like an unseen item. Some techniques include SIngular Value Decomposition (SVD), Non-Negative Matrix Factorization (NMF) and Probabilistic Matrix Factorization (PMF).


**Proposed Hybrid Methods & Noval Approaches:** xLSTM (extended LSTM) incorporates architectural enhancements like attention mechanism, gating improvments and bidirectional capabilities. It will be impactful due to several unique aspects when to compared to the traditional successful methods. 


First Let's start with basic example, to get started:
----------------------------------------------------------------------------------------------------------------
Lets say, we have three best friends, and all of them were having equal knowledge but totally different varities of interests:

As a New User (Product/Service Buyer), may likes **Football, Hiking, Climbing, Animal Caretaking and Reading**

Friend A (Existing user A): Enjoys **Football, Hiking, Running, Animal Caretaker and Climbing**

Friend B (Existing user B): Prefer Singing, Writing and Reading.

Friend C (Existing user C): Likes Bicycling and Singing.  

----------------------------------------------------------------------------------------------------------------

Take this as an simple example, Clearly,  **Friend A** has similar interest more similar to new user and we would **assign more weightage ** to him/her, right ?. In neural networks it called "weights". 

Now, its just about three friends with eight different interest, which is easier for calculations. What would be the case if we have 100 million users and all of them were having 50,000 different varities of interesting data points. Then we may need to leverage the latest techniques. 

![image](https://github.com/user-attachments/assets/a102eda4-475a-42f1-a692-e90480215c5e)

![image](https://github.com/user-attachments/assets/937a996b-487a-436b-8329-4b950d9cfad1)

Singular Value Decomposition: (SVD to decompose the original matrices into three smaller matrices)
![image](https://github.com/user-attachments/assets/50bac5cb-eae8-44f2-8ca0-270a69233eef)
*Slight variations in the input matrices noted.


Take Away from SVD:

1. Higher positive values in the reconstructed matrix indicate stronger recommendations.

2. For users or hobbies not strongly represented, values will remain closer to 0 or negative.

In this case, (User to User): the horse buyer has atleast a good co-relation with User A (0.55 is a good start).

Additionally (Content to Content) we can even recommend user A for "Reading", because of higher positive value (i.e. 0.96, refer last matrices User A and they doesn't have this habit of reading already).  

It's a basic example and there are some drawbacks associated with it, like sparse zero values, curse of dimensionality and other limitations.

Value Proposition: The core concept and unique benefit is still the same **recommend the best similar product/service to the end user** and to help them. 

It is also estimated that the **market scope** for recommender system is expected to be approx 20-28 billion by 2030, currently in 2024 valued approx 6 billion US dollers. 

Below are the two major types in Recommenders:
1. Collaborative Filtering (User to User), and
2. Content Based Filtering (Product to Product).

Different Simple methods to identify user similarities:
1. Correlations, 2. Cosine Similarities, 3. Jaccard Similarities, 4. Euclidean Distance, 
5. Hamming Distance, 6. Manhatten Distance, 7. Bhattachryya Distance,
8. Neural Network Embeddings (Collaborative Filtering),
9. Kullback Leibler divergence, 10. Embeddings and Latent Features, 11. Sequence-Based Similarity,
12. Deep Collaborative Filtering with Embeddings (via Neural Networks),
13. Transformer Models for Sequential Recommendations (e.g. BERT4Rec), 
14. In life science application (some techniques used for DNA Sequencing to find the similarities, which could also be leveraged for RS), and
15. Other Hybrid Approches.

**Data Sources:** Here, we will be leveraging RecBole libraries to explore various models and to develop more customizable one. 

List of Different Varieties of Datasets: (Ref: https://recbole.io/)

![image](https://github.com/user-attachments/assets/e842adf0-6eaa-48b7-9ffa-68312db0788e)

**Results:** Comparision and Performance Results For All Approaches:
1st set of results for the simple BPR model with 10 epochs, for movielens datasets: (To be fine tuned further)

![image](https://github.com/user-attachments/assets/d2bf1736-6617-4afc-9dbe-88134e8e40fe)

In machine learning, **epochs** tells us how many times we process our complete data until we reach final/optimum goal.  And, how fast did we adjust our weights to reach that optimum level is called **learning rate** (Usually it's like 0.01, 0.001 etc). 

Cold Start Problem (For new users): TBA

![image](https://github.com/user-attachments/assets/d157ae60-54c2-41e8-9bf3-e79e1250bc1b)


**Recbole - Major Classifications:**

Four Classifications: 

1. General Recommendation (GR): Netflix use case which we discussed above. The interaction of users and items is the only data that can be used by model. Trained on implicit feedback data and evaluated using top-n recommendation. Collaborative filter (CF) based models are classified here. 

2. Content-aware Recommendation: Amazon use case. Click-through rate prediction, CTR prediction. The dataset is explicit and contains label field. Evaluation conducted by binary classification.

3. Sequential Recommendation: Spotify, similar to time series problem, which we discussed earlier. The task of SR (next-item recommendation) is the same as GR which sorts a list of items according to preference. History interactions are organized in sequences and the model tends to characterize the sequential data. Session-based recommendation are also included here.

4. Knowledge-based Recommendation: Knowledge-based recommendation introduces an external knowledge graph to enhance general or sequential recommendation.

SEO (Search Engine Optimization) and SEM techniques may also be merged, along with Google Adsense and adwords, to improve user experience further. 


**Scope** For Recommendation Engines In Various Sectors:
1. Energy Sectors, (Energy Saving Programs, Substations, CO2 Emission, Solar, Grid Automation, Sensor Meters, Electrical Products and HVAC transmission)
2. Banking and Fintech sectors, (Wealth Management, Customized Credit Products, Investment Portfolio's, Equities, and Insurance plan recommendations)
3. Technology and Service sectors, (Ecommerce Products)
4. Entertainment and Gamification, (Custom Localization and Immersive Experience)
5. Food, Beverages & Agriculture Industry (AI-based recommendations for improved crop yield, agricultural products, custom fertilizers, supply and demand forecasting, as well as weather and climate change insights using satellite data.)
6. Healthcare and Pharmaceutical, 
7. Aviation and Transportation, and 
8. Other Specialized Sectors. 

**Evaluation Metrics:** To evaluate the model accuracy Recall 5, 10, Precision, NDCG will be used mainly. 

Recall = How many relevant items recommended/Total No. of relevant items **available**

It measures the relevance. 

Precision: How many relevant items recommended//Total No. of items **recommended**

It measures the accuracy.

**Normalized Discounted Combined Gain (NDGC):** For Ranking.


**Few Hugging Face models to be tested:**
1. Transformers4Rec by NVIDIA: Integrates with Hugging Face Transformers, enabling the application of transformer architectures to sequential and session-based recommendation tasks.
                  transformer_config = tfr.TransformerBlock(
   
                   d_model=64,  # Embedding dimension
   
                   n_head=4,    # Number of attention heads
   
                   num_layers=2  # Number of transformer layers)

           Embedding dimension, Attention Heads, Transformer layers - Working examples to be added

3. RecGPT: RecGPT is a domain-adapted large language model specifically trained for text-based recommendation tasks.

**References:**

[1] xLSTM: Extended Long Short-Term Memory: https://arxiv.org/pdf/2405.04517

[2] xLSTM-Mixer: Multivariate Time Series Forecasting by Mixing via Scalar Memories: https://doi.org/10.48550/arXiv.2410.16928

[3] Amazon Science: https://github.com/amazon-science

[4] xLSTM Time : Long-term Time Series Forecasting With xLSTM: https://doi.org/10.48550/arXiv.2407.10240

[5] Quaternion Transformer4Rec: Quaternion numbers-based Transformer for recommendation: https://github.com/vanzytay/QuaternionTransformers

[6] Recommender Systems: A Primer: https://doi.org/10.48550/arXiv.2302.02579

[7] Exploring the Impact of Large Language Models on Recommender Systems: An Extensive Review: https://arxiv.org/pdf/2402.18590

[8] Recommender Systems with Generative Retrieval: https://openreview.net/pdf?id=BJ0fQUU32w

[9] Attention Is All You Need: https://arxiv.org/abs/1706.03762

[10] Recbole: https://recbole.io

[11] Group Lens: https://grouplens.org/datasets/movielens/100k/

[12] OpenAI: https://openai.com/

[13] Hugging Face: https://huggingface.co/docs/hub/en/models-the-hub

[14] Kreutz, C.K., Schenkel, R. Scientific paper recommendation systems: a literature review of recent publications. Int J Digit Libr 23, 335–369 (2022). https://doi.org/10.1007/s00799-022-00339-w

[15] Recommendation Systems: Algorithms, Challenges, Metrics, and Business Opportunities https://doi.org/10.3390/app10217748

[16] Roy, D., Dutta, M. A systematic review and research perspective on recommender systems. J Big Data 9, 59 (2022). https://doi.org/10.1186/s40537-022-00592-5

[17] A Comprehensive Review of Recommender Systems: Transitioning from Theory to Practice https://doi.org/10.48550/arXiv.2407.13699



   
