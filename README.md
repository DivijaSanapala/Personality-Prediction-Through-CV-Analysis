# Personality-Prediction-Through-CV-Analysis

The proposed method would make it easier to shortlist candidate CVs from a large
number of applications while maintaining consistent and fair CV ranking criteria. The proposed
algorithm will rate the experience and key skills necessary for a certain job position based on the
CV analysis and the results from the aptitude tests. Based on this the recruiters can make a
decision on the most suitable candidates for the job position. This method will make it easier for
the HR department to shortlist candidates using CV analysis and aptitude tests.

## Flow chart Explaining the Implementation

<img width="142" alt="Screenshot 2022-10-08 203550" src="https://user-images.githubusercontent.com/79396759/194718066-3df5db9a-0a51-4bd3-85d0-ec22eca08f8e.png">

The main goal of this project is to provide a platform open to the recruiters of an organization for ease in
recruiting. This system helps them save so much time and effort as they don’t have to go through
many CVs but rather see a summarized version, giving everybody a fair chance of showcasing
themselves and not having their CV gone unread. The system allows recruiters to not only see
candidates resumes but also their personality type after they’ve answered a set of
personality-based questions. This helps them identify the ideal candidate with the qualities they
15 were looking for. 

The dataset is used from Kaggle for Resume dataset and Personality Test dataset. The scores of the psychometric test of personality questions is analyzed. The first 50 columns (that is 10 questions for each of the 5 personality types) are clustered into 10 batches
using the K-means algorithm. Then each of the 5 personality types is given a weight by the score
it gets from the question answered. Then all the scores are aggregated and normalized using min-max normalization. 10 clusters are generated as follows:

Cluster 1 - INFP (The Mediator) Introvert, Intuitive, Feeler, Perceiver,
Cluster 2 - ENTP (The Debator) Extrovert, Intuitive, Thinker, Perceiver,
Cluster 3 - ENTJ (The Commander) Extrovert, Intuitive, Thinker, Judger,
Cluster 4 - ENFJ (The Protagonist) Extrovert, Intuitive, Feeler, Judger,
Cluster 5 - ENFP (The Campaigner) Extrovert, Intuitive, Feeler, Perceiver,
Cluster 6 - ISFJ (The Defender) Introvert, Sensor, Feeler, Judger,
Cluster 7 - ESFJ (The Consul) Extrovert, Sensor, Feeler, Judger,
Cluster 8 - INFJ (The Advocate) Introvert, Intuitive, Feeler, Judger,
Cluster 9 - ISFP (The Adventurer) Introvert, Sensor, Feeler, Perceiver and 
Cluster 10 - ESTP (The Entrepreneur) Extrovert, Sensor, Thinker, Perceiver
