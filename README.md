# Machine Learning Project
## Branch - Duarte Valente

### Important Notes and comments for my team

- Data Visualization, Feature Engineering & Preprocessing

1. I don't really care much what we do here. I believe you guys did a fine job.
2. I don't mind having `Age` as a category or not having the `isPureBreed` as a binary value.

- Supervised Learning

1. I don't care which models we use. Just that we use them properly.
2. I would rather you use the format I am using rather then yours.
3. I **dislike** the way you are showing the results, **expecially** the confusion matrix. I have never seen anyone creating 2 confusion matrixes, one for the training data and other for the test. The only one we should be computing to begin with is the `test-split`.
4. Copy my `SMOTE`. If you don't set the `sampling_strategy` it will default to 1, meaning it will create fake data intil the proportions are 1:1. This is bad because by doing this we are creating a large amount of fake data and we don't need the proportions to be 1:1 to diminish the imbalancing problem. If we get the proportions to 7:10 should be more then enough.
5. Use your `KNN`. I shouldn't have created the elbow method although its probably not a big deal. Use a range between 3 and 21 Ks
6. I would like to use one ensemble method. The one I picked was `Random Forest`. Basically it creates a forest instead of a single tree. All trees get to be tested and the best one from the forest is the one used. Could be cool if we still had the `Decision Tree` model to compare results. Normally Random Forest will always have a better results, its just a matter of 'is it worth it' when it comes to the improvement vs complexity.
7. Regarding f1 weighted for multiclass classification. I like it as an alternative to using SMOTE.

- Unsupervised Learning

I didn't dwelve into this myself just took a quick look at Alexandre's work, but here are some takes you might want to consider.

1. Why are we using silhouette score instead of others like BIC or AIC?
2. Do you guys want to create a new non-supervised model like PCA? Could be insteresting to check feature importance and add to feature engineering.

- Final Results

1. Don't hate the fact that you are explaining what the F1 score is.
2. I like you comparing results to base model.

# Side Notes

No teu bloco 76 fazes o comentario de que experimentaste remover as vars mas o resultado n melhorou.

Remover vars e n perder performance = melhorar. Quanto mais simples melhor!
