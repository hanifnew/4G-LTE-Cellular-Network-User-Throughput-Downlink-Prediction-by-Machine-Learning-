# 4G LTE Cellular Network User Throughput-Downlink Prediction by Machine-Learning
Final Capstone Project
##### Muhammad Hanif Naufal Eka Wiratama 

# Business Understanding
### Background
*Record any known information about the business situation at the start of the project. Is there already a solution in place? Describe any solutions in place and why they are seeking a new solution. What should the new solution improve?*

1. Over the years, there has been a significant increase in mobile network traffic. LTE will remain the dominant cellular access technology by number of subscriptions for now. During the 3rd quarter of 2020, LTE users increased by approximately 70 million and reached a total of approximately 4.5 billion users, or equal to 57 percent of all cellular subscriptions.

    (Ericsson AB, “Ericsson Mobility Report,” Ericsson AB, 2020.)

2. Advances in wireless communication technology have brought broadband speeds directly to smartphones, allowing mobile users to access high-speed Internet services such as online gaming and video streaming. This significantly increases the load on the cellular network, and causes throughput to fluctuate significantly in network traffic.

    (A. Samba, Y. Busnel, A. Blanc, P. Dooze, and G. Simon, “Instantaneous throughput prediction in cellular networks: Which information is needed?” in 2017 IFIP/IEEE Symposium on Integrated Network and Service Management (IM). IEEE, pp. 624–627.)

3. Based on previous research on network utilization, it is stated that accurate prediction of user throughput can significantly increase bandwidth utilization.

    (X. K. Zou, J. Erman, V. Gopalakrishnan, E. Halepovic, R. Jana, X. Jin, J.Rexford, and R. K. Sinha, “Can accurate predictions improve video streaming in cellular networks?” in Proceedings of the 16th International Workshop on Mobile Computing Systems and Applications, (2015), pp. 57–62.)

4. ML has been applied successfully in the area of mobile networks, including assisted mobile network planning techniques for analyzing big data in mobile network
    (Y. Liu and J. Y. B. Lee, "An Empirical Study of Throughput Prediction in Mobile Data Networks," 2015 IEEE Global Communications Conference (GLOBECOM), 2015, pp. 1-6, doi: 10.1109/GLOCOM.2015.7417858.)

### Our Method

*   to predict the future downlink throughput of the UE
*   to visualize the throughput prediction result 
*   to compare some of machine learning predictor performance based on throughput prediction
*   to guide telco expert how to predict the throughput based on their own-dataset

### Problem Statements dan Goals

Based on some of the information described before, we will develop a web app-based throughput prediction dashboard to answer the following problems. From a set of features that will exist, 

* Which features can predict the future downlink throughput of the user equipment? 
* Which features can measure the performance of 4G LTE network 
* Which features can visualize the throughput prediction result?
* Which features can compare some predictor method’s performance?
* Which features can guide telco experts how to predict the throughput based on their own-dataset?
 
To answer these questions, predictive modeling will be made with the following goals or objectives:

* Find out the features that can predict the future downlink throughput of the user equipment
* Find out which features are most correlated with the 4G LTE network performance
* Find out the features that can visualize the throughput prediction result
* Find out the features that can compare some predictor method’s performance
* Find out the features that can guide telco experts how to predict the throughput based on their own-dataset
* Create a machine learning model that can predict the future downlink throughput of the user equipment as accurately as possible based on existing features.

### Methodology

Network performance prediction is the goal to be achieved. As we know, there are many parameters that are used to see the performance of the network, and all of them are continuous variables. In predictive analytics, making a continuous variable prediction means that you are solving a regression problem. Therefore, the methodology in this project is: to build a regression model with the network parameter as the target.

### Metric

Metrics are used to evaluate how well your model predicts network parameters. For the case of regression, some metrics that are usually used are Mean Squared Error (MSE) or Root Mean Square Error (RMSE). In general, this metric measures how far the predicted result is from the actual value. We'll go into more detail about these metrics in the Evaluation module.

The model development will use several machine learning algorithms, namely Support Vector Regression (SVR),  K-Nearest Neighbor (KNN), Ridge Regression, Random Forest, and Boosting Algorithm. From these five models, one model will be chosen which has the smallest predictive error value. In other words, we will make the model as accurate as possible, that is, the model with the smallest possible error value.

Creating predictive models with machine learning requires data. The good news is, we have the data that we need to build predictive models from the previous research. The dataset that we will use in this practice is the 4G LTE User Equipment Measurements along Kingston Transit 502 Bus Route dataset. The explanation of the dataset used will be explained in the next section.
