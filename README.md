# Big-Data-Analysis

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: HARISH AADITYA SRIDHARAN

*INTERN ID*: CT1MTDL12

*DOMAIN*: DATA ANALYTICS

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH


In this task, we utilized PySpark, a Python API for Apache Spark, to conduct a comprehensive data analysis on the Titanic dataset. The Titanic dataset, often used in data science and machine learning exercises, contains information about passengers aboard the Titanic, including whether they survived or not. This task aimed to demonstrate the use of big data tools like PySpark for analyzing large datasets, processing them efficiently, and generating valuable insights.

Titanic Dataset Overview
The Titanic dataset consists of various columns that provide details about passengers, such as their age, sex, class (Pclass), fare, siblings/spouses aboard (SibSp), parents/children aboard (Parch), and the embarked port (where they boarded the Titanic). The key column in the dataset is Survived, which indicates whether a passenger survived (1) or perished (0) during the sinking of the ship. This dataset has been widely used for predictive modeling, specifically for tasks like survival prediction.

The Titanic dataset includes the following key columns:

PassengerId: Unique identifier for each passenger.

Pclass: Passenger class (1st, 2nd, 3rd).

Name: Name of the passenger.

Sex: Gender of the passenger.

Age: Age of the passenger.

SibSp: Number of siblings or spouses aboard.

Parch: Number of parents or children aboard.

Fare: Ticket price.

Embarked: Port of embarkation (C = Cherbourg; Q = Queenstown; S = Southampton).

Survived: Survival status (0 = No, 1 = Yes).

Using PySpark for Big Data Analysis
Apache Spark is a powerful distributed computing framework that can handle big data efficiently. PySpark is the Python API that allows Python developers to use the features of Apache Spark, making it easier to work with large datasets. While the Titanic dataset is not large by big data standards, using PySpark demonstrates how easily you can scale the data processing pipeline to handle larger datasets in the future.

The primary advantage of using PySpark for this analysis is its ability to process large datasets in a distributed manner, where the computations are parallelized across multiple nodes. This makes it much more efficient than traditional data analysis methods, especially when dealing with massive datasets that would otherwise be difficult to handle using just a single machine.

Steps Taken in the Analysis
Setting up the PySpark Session: The first step involved initializing a Spark session using SparkSession.builder.appName("Titanic Big Data Analysis").getOrCreate(). This session allowed us to interact with the Spark cluster and initiate the data processing tasks.

Loading the Titanic Dataset: The Titanic dataset was loaded into PySpark using spark.read.csv(), which reads the CSV file into a DataFrame. PySpark automatically inferred the column types (integer, float, string) using the inferSchema option. This DataFrame allowed us to perform various data processing tasks.

Data Exploration: We explored the dataset using df.printSchema() to print the schema of the DataFrame, and df.show(5) to display the first five rows of the dataset. This step helped ensure that the dataset was loaded correctly.

Data Cleaning: The dataset had missing values in some columns, and we needed to clean it. We dropped rows with missing Age values and filtered out rows where Fare was less than or equal to zero. This helped make the data ready for analysis.

Performing Data Analysis: We conducted several analyses:

Survival Rate by Gender: We grouped the data by sex and calculated the survival rate for each gender. This analysis showed that females had a higher survival rate than males.

Survival Rate by Passenger Class: We grouped the data by Pclass and analyzed the survival rate for passengers in 1st, 2nd, and 3rd classes. First-class passengers had the highest survival rate.

Average Age by Survival Status: We analyzed the average age of passengers who survived and those who didn’t. This analysis revealed that younger passengers had a higher chance of survival.

Insights and Conclusions: The analysis provided several valuable insights:

Females had a significantly higher survival rate than males.

Passengers in the first class had the highest survival rate, followed by second and third classes.

Younger passengers, on average, had a better chance of survival than older passengers.

Conclusion
This task showcased the use of PySpark for handling big data, even though the Titanic dataset itself is relatively small. By using PySpark, we efficiently loaded, cleaned, and analyzed the data, demonstrating how Spark's distributed nature can be leveraged for big data processing. While the Titanic dataset provided a small-scale example, the techniques used here can easily be scaled up to handle larger, more complex datasets.

PySpark allows data scientists to work with large datasets by providing high-level APIs for data manipulation, aggregation, and analysis. This task served as an excellent introduction to the power and scalability of PySpark, demonstrating how even small datasets can benefit from the distributed processing power of Spark. With its ability to scale horizontally, PySpark is an ideal tool for handling much larger datasets in future big data analysis tasks.

#OUTPUT

![Image](https://github.com/user-attachments/assets/7dc64abc-094c-4d4c-bd27-43f29365f6ad)
