# Time-Series-Analysis
CS 535/CS435
Fall 2018
Semester Long Project
Assigned on 22 August 2018
Final Due on 10 December 2018

Total Points: 100


This is a semester-long project, encouraging students to dive into the research in data mining. Specifically, this project concerns with the research in two parts, one with a presentation and the other with an implementation, both on the topic of time-series prediction. The project has three phases. The first phase is for the research and the coding part, the second phase is for the presentation of your research and implementation as well as the experiments, and the final phase is for turning in the presentation materials. 

In this project, you are asked to study the general topic of time-series data mining, and specifically for time-series data trend prediction. Note that this is not a new topic in the literature, as studies were already around even way before the official advent of data mining research (e.g., in the literature of control theory or pattern recognition). On the other hand, in the literature of data mining, time-series data mining is considered as one of the advanced topics and has many important and hot applications in the real-world such as e-commerce, stock analysis, and weather forecast.

The specific problem in this project is about the time-series data trend prediction. The specific application scenario is in e-commerce. You are given a real dataset obtained from a real-world e-commerce application where there were 1000 products and 31490 customers (i.e., buyers) who bought these products. Of these 1000 products there are 100 key products (popular products). Also these 1000 products are in 15 categories. The specific data are given in the seven files and the specific details of these files are given below. The time window of this dataset is in 118 days with data documentation for each day. Hence, the time unit is one day where the timeline goes from the 0-th day to the 117-th day (17 weeks less one day in total). Now you are asked to do the sale quantity prediction for the 100 key products for each day between the 118-th day and the 146-th day (29 days).

•	buyer_basic_info.txt: the basic attribute information of the buyers; in particular, the column names of this table are "buyer_id", "registration_time", "seller_level", "buyer_level", "age", and "gender". If we do not know the gender of a buyer, we set this buyer’s gender attribute as -1.

•	buyer_historical_category15_quantity.txt: the consumption quantities in the 15 categories for the buyers; in particular, the column names of this table are "buyer_id", "consumption quantity in the 1st category", ..., and "consumption quantity in the 15th category". The 15 categories are the ones of the products the customers bought in this dataset.

•	buyer_historical_category15_money.txt: the consumption amounts in the 15 categories for the buyers; in particular, the column names of this table are "buyer_id", "consumption amount in the 1st category", ..., and "consumption amount in the 15th category".

•	product_features.txt: the basic attribute information of the products; in particular, the column names of this table are "product_id", "attribute_1", "attribute_2", and "original price".

•	Key_product_IDs.txt: the key product IDs

•	trade_info_training.txt: the trade information between the key products and the buyers from the 0-th day to the 117-th day; in particular, the column names of this table are "product_id", "buyer_id", "trade_time", "trade_quantity", and "trade_price".

•	product_distribution_training_set.txt: there are 119 columns, where the 1-st column shows the "product_id" and the 2-nd to the 119-th columns show the "quantities" of the key products from the 0-th day to the 117-th day; for example, the element at the 5-th row and the 10-th column in this table shows the quantity of the 5-th product at the 8-th day.

For undergrad students you are only asked to do the prediction for the overall sale quantity of the 100 key products for each day of the time window from the 118-th day to the 146-th day, while for grad students you will need to do the prediction for the sale quantity not only for the overall sale but also for each key product for each day of the time window. 

You will receive the assignment of the presentation schedule after the course registration is closed.

The first phase begins when you have received the assignment. This phase concerns with the implementation of a time-series prediction method that you either take from the literature or you have developed by yourself as the result of your research in the this phase. You may use any programming language to implement the method and you may also use any existing libraries.

The first phase begins at the beginning of the semester, and the due time of turning in the coding results is 11:59pm on 12 November (NOT 10 December). Please make sure to follow the format requirement as the text output file specified here. The file puts each prediction as one line where the first prediction is for the overall prediction and each subsequent prediction is for a key product. Each prediction output line begins with the key product id where the overall prediction id is 0. There is a space between the prediction and the key product id. Then there is a space between a pair of the predictions of two neighboring days. The prediction lines in the output file begin with the first line as the overall prediction where the product id is 0, and then the first key product prediction with the smallest product id (i.e., 1), all the way to the last line as the prediction for the last key product prediction (i.e., id = 964). Also note that for undergrad students your output file only has one line prediction just for the overall prediction beginning with the product id = 0.

The second phase concerns with the presentation of your research as well as the implementation and experiments. This phase begins on 26 November. You must complete the preparation for the presentation before the assigned presentation date and give your presentation on your research on the assigned presentation date. You are given 5 minutes for the presentation. In the presentation, you must give the following information:

•	Explain conceptually what time-series data mining is about
•	Describe the specific problem and the specific method you have implemented or developed as a solution to the problem you are given
•	Report your implementation results in the prediction

Please make sure that your presentation cannot exceed 5 minutes or you will be subject to penalty. I will then give a grade on your presentation part of the project.

The third phase is to turn in your presentation slides to myCourses by the noon on 10 December. 

What you need to turn in for the coding part: you shall turn in a zipped package containing the source code of your implementation of the prediction method with appropriate comments and documentations in the code, a README file to explain how to compile and run your code under what specific environment, and a text file containing the output matrix following exactly the format requirement stated above. 

A final note: you must complete this project, for all the three phases, independently and no collaboration is allowed.




