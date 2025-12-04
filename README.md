# Swire Cart Abandonment

## Business problem and project objective

Swire Coca-Cola has introduced a new digital ordering platform, MyCoke360, which launched in summer 2024. Swire, like many other companies that deal with online ordering, has to worry about cart abandonment. Cart abandonment is defined as when a customer adds an item to their MyCoke360 cart and does not make a purchase by
their next order date. Cart abandonment can result in delayed purchases and a loss of revenue. The goal of this project is to identify the behavioral events or sequences of events that most influence a customer's decision to abandon their cart. These events will be identified through creating a model that predicts cart abandonment. The model will use Google Analytics and order data as input data. Examining the model's results and the most significant factors in the predictions will help identify the key factors influencing customer behavior, which can then be used to create insights that improve order completion and reduce revenue loss. 

## My group's solution to the business problem

Our solution included a logistic regression and a random forest model, with the features as summarized user actions. Both had extremely high AUC scores, 0.895 and 0.98, respectively. Both of these high AUC scores suggest overfitting and possible data leakage, which is something we would've liked to deal with had we been given more time. These models found that heavy browsing without purchasing and removing items after having added them to the cart are the highest predictors of cart abandonment. Heavy browsing led to a customer being 26 times more likely to abandon their cart, and removing items after adding was 4.5 times more likely to abandon. Based on these top predictors, we came up with three recommendations to help improve order completion. First, create a live chat for those who may be unsure about what they need to buy. Second, check out reminders for anyone who has added items to their cart but has not purchased after a certain period of time. Third, simplify the MyCoke360 user interface to minimize the number of steps in the entire checkout process, creating a smooth process where the customer will have fewer sticking points. 

## My contribution to the project

I helped clean the data and do EDA. I was also responsible for combining the orders dataset and Google Analytics data to make sure all orders were present when creating order windows. I created a performance benchmark model and a decision tree model. For both the group EDA and Modeling notebooks, I organized the notebooks, bringing all three group members' code together. 

## Business value of the solution


