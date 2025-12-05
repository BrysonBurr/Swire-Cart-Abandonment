# Swire Cart Abandonment

## Business problem and project objective

Swire Coca-Cola has introduced a new digital ordering platform, MyCoke360, which launched in summer 2024. Swire, like many other companies, has to worry about cart abandonment. Cart abandonment is defined as when a customer adds an item to their MyCoke360 cart and does not make a purchase by their next order date. Cart abandonment can lead to delayed purchases and revenue loss. The goal of this project is to identify the behavioral events or sequences of events that most influence a customer's decision to abandon their cart. These events will be identified through creating a model that predicts cart abandonment. The model will use Google Analytics and order data as input data. Examining the model's results and the most significant factors in the predictions will help identify the key factors influencing customer behavior, which can then be used to create insights that improve order completion and reduce revenue loss. 

## My group's solution to the business problem

Our solution included a logistic regression and a random forest model, with the features as summarized user actions. Both had extremely high AUC scores, 0.895 and 0.98, respectively. Both of these high AUC scores suggest overfitting and possible data leakage, which is something we would've liked to deal with had we been given more time. These models found that heavy browsing without purchasing and removing items from the cart are the highest predictors of cart abandonment. Heavy browsing led to a customer being 26 times more likely to abandon their cart, and removing items was 4.5 times more likely to result in abandonment. Based on these top predictors, we came up with three recommendations to help improve order completion. First, create a live chat for those who may be unsure about what they need to buy. Second, check out reminders for anyone who has added items to their cart but has not purchased after a certain period of time. Third, simplify the MyCoke360 user interface to minimize the number of steps in the entire checkout process, creating a smooth process where the customer will have fewer sticking points. 

## My contribution to the project

I helped clean the data and do EDA. I was also responsible for combining the orders dataset and Google Analytics data to make sure all orders were present when creating order windows. I created a performance benchmark model and a decision tree model. For both the group EDA and Modeling notebooks, I organized the notebooks, bringing all three group members' code together. 

## Business value of the solution

While our solutions don't provide direct financial impact, such as an increase in revenue, our insights can provide directions that Swire can take to improve MyCoke360. Identifying that heavy browsing without purchasing and removing items from the cart are patterns that lead more to cart abandonment indicates that the customer experience on their platform needs to be improved. This could be achieved through checkout reminders, live chats, and a simplified user interface, all of which have the potential to improve order completion and reduce revenue loss. 

## Difficulties encountered along the way

There were two main challenges we faced during the project. The first was creating the order windows for each customer. That required combining multiple columns from 4 different datasets. Customer policies also didn't stay consistent, which added another layer of complexity in creating an order window. All of the factors made it difficult for us to calculate precisely when a customer should order next. The other challenge we encountered was data leakage. Our AUC scores, which I reported in the group's solution section, indicate that there was overfitting and data leakage. There are certain behavioral events or sequences of events that are reflective of cart abandonment. This leads to our models not learning from predictive signals as they should. With more time, we would've liked to explore more about what events needed to be removed so that data leakage isn't a problem.

## What I learned in the project

In this project, I learned how to work with messy, real-world data. It was a very helpful experience working with data where the target variable, in this case, order windows, had to be created and was not already given to us. I also learned about the importance of data quality and how important it is to be thorough when evaluating and preparing the data for modeling. While we spent a lot of time cleaning and preparing the data to ensure it was clean for modeling, we were not quite thorough enough, as we encountered data leakage. As a result, it became harder to trust the models we built and the results that came with them. From this, I've learned to think more carefully about where data leakage might occur and how to prevent it so that I can trust the models that are built.  
