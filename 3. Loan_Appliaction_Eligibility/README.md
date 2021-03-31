## Loan Application - Repayment Capability

### 1. Introduction
About twenty years ago, personal loan is a thing that is very complicated in terms of the application process. It takes so much to process every loan application because they are do it manually through a loan analyst. But right now, there are so many companies that are offering a simple and quick loan application. So how do they do that? Did they force their loan analyst to work quick?. If no, who's do that? Yeah 'Machine Learning'. With machine learning we're be able to process the loan application quickly without having to analyze the entire application. We can train the machine learning model with a previous loan application data how to predict whether an applicant can repay the loan or not based on their profile.

So this project is aim to make some machine learning model to predict if an applicant is able to repay the lending company or not. The model is just a basic classification model such as logistic regression, support vector machine, decision tree, and random forest. I will use Python for coding and Jupyter Notebook as the IDE for running the program.


### 2. Data and Preprocessing
Data is a business real case from a finance firm. The data consist of 4 csv file, app_train.csv, app_test.csv, prev_app.csv, and installment_payment.csv. The file app_train.csv and app_test.csv contain information about loan and applicant at application time, those already separated in train and test file data. The file prev_app.csv contains information about previous loan application data and installment_payment.csv contains information about past payment data. Each of the file data contains a loan id as the id of each application. Also in prev_app.csv and installment_payment.csv, there are previous loan id of each applicants, so for every applicants who applied their loan, there is a record for their previous application data, means that every loan id has one or more previous application id. So, for those two data (prev_app.csv and installment_payment.csv), we can generate a derivative feature from it besides the features from the main dataset (app_train.csv and test_train.csv).

For prev_app.csv data, a derivative feature can be extracted called APPROVED_SCORE based on the CONTRACT_STATUS of previous application data, is it 'Approved', 'Refused', 'Cancelled', or 'Unused offer'. The smaller the score, the more likely the costumer loan application will be approved and vice versa (this is mean to get the positive correlation with the target variable because 0 it means the more likely the costumer will repay the loan). So we make a score vocabulary based in the each CONTRACT_STATUS. This score based on the assumptions that costumers with Unused offer status and Cancelled status has a particular meaning.



### 3. Feature Selection

### 4. Models

### 5. Results

### 6. Discussion
