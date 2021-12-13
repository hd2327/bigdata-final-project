# bigdata-final-project
NYU CS-GY 6513 Big Data Group 20

Group member : Hao Dong hd2327 / Siwei Wang sw5050 / Yinchen Shi ys4653

There is a github repository for this project: https://github.com/hd2327/bigdata-final-project. The relate document and simple description are as follows:

1. data_reference : the reference data we commit to https://github.com/VIDA-NYU/reference-data-repository
- reference_data_NYC zipcode.csv : NYC zipcodes
- reference_data_collision factor.csv : factors of collisions
- reference_data_vehicle.csv : types of vehicles

2. data_analysis.zpln : the data analysis file with Spark, please open by **zepplin**

3. data_cleaning_improve.ipynb : the data cleaning file after improvement, please open by **jupyter notebook**

4. data_visualization.ipynb :  the data visualization file with Spark and Matplotlib, please open by **jupyter notebook**

5. report.pdf : the report

# how to open
At first，we should run **data_cleaning_improve.ipynb** in jupyter notebook to get the result after cleaning. The output is out.zip and there is a file named out.csv.

Then we need put the out.csv to HDFS on the Peel cluster by command *hfs -put out.csv*. Then we need update the code in **data_analysis.zpln** and run it in school zepplin environment.

The code to be modified is parking_v = sc.textFile("/user/hd2327/data_cleaning_output.csv"). The hd2327 is my netid. After that, the data_analysis.zpln can run.

In the end, open **data_visualization.ipynb** and run it in jupyter notebook to look at the result.
