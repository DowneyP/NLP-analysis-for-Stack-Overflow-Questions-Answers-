# NLP-analysis-for-Stack-Overflow-Questions-Answers-
This is Natural Language Process analysis for Stack Overflow Questions and Answers.



##########################################################################################

Questions Clustering for Stack Overflow

 Agenda
 **Project Background**
 
 About Stack Overflow:
- A question and answer site for professional and enthusiastic programmers
- Over 18 million questions posted covering a wide range of topics in computer programming
Objectives:
Based on a ready dataset of questions and answers on Stack Overflow, we intend to:
- Detect recent popular topics or recognize topic trends over time
- Analyze attributes of Q&A on different topics
Techniques:
- Integrated use of NLP techniques obtained from the class
- Questions clustering mainly through Topic Modelling
Guiding significance:
- Identify user needs and expectations
- Help manage the community and improve recommendation system

**Data Description & Preparation**

Data Description:
Datasets include 10% of questions and those corresponding answers from the Stack Overflow programming Q&A website.
- Questions: contains (Question)Id, OwnerUserID, CreationDate, ClosedDate, Score, Title and Body The Id column refers to all non-deleted Stack Overflow questions whose Id is a multiple of 10.
- Answers: contains (Answer)Id, OwnerUserID, CreationDate, ParentId, Score and Body The ParentId column links to the Questions file as (Question Id).
- Tags: contains (Question)Id and Tag on each of these questions
People can provide the tags related to the question on their own or Stack Overflow can predict the tags using the text in title and description. We assume tags here refer to the former one.
Data Preparation:
- Turn Questions.CSV file to Questions.JSON file, and break down on yearly basis
- Basic text processing: Remove Stopwords, Punctuations...

**Research Questions**

Q1. What were the popular topics among 2008 - 2016 questions?
- Questions file and Tags file
- Using LDA Topic Modeling
Q2. What was the yearly trend for the 4 programming languages (Python, Java, SQL, C#)?
- Questions file
- Using Word2vec Taxonomy to do topic classification
Q3. Is there any correlation between the length of question/answer and its score?
- Answers file & Questions file & Tags file
- Summarize question body for title recommendation; apply linear regression for correlation analysis

**Methodologies 4 & Findings**

Listed in the PDF - "Methodologies and Findings"

##########################################################################################
--Published at 9 Nov by Downey

