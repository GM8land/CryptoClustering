
## Module 11 Challenge: Crypto Clustering 
### Instructions
Utilize K-means algorithm and principal component analysis (PCA) to classify cryptocurrencies according to their price fluctuations across various timeframes 
### Requirements
- Find the Best Value for k Using the Original Scaled DataFrame (15 points)
To receive all points, you must:
  - Code the elbow method algorithm to find the best value for k. Use a range from 1 to 11. (5 points)
  - Visually identify the optimal value for k by plotting a line chart of all the inertia values computed with the different values of k. (5 points)
  - Answer the following question: What’s the best value for k? (5 points)
- Cluster Cryptocurrencies with K-Means Using the Original Scaled Data (10 points)
To receive all points, you must:
  - Initialize the K-means model with four clusters by using the best value for k. (1 point)
  - Fit the K-means model by using the original data. (1 point)
  - Predict the clusters for grouping the cryptocurrencies by using the original data. Review the resulting array of cluster values. (3 points)
  - Create a copy of the original data, and then add a new column of the predicted clusters. (1 point)
  - Using pandas’ plot, create a scatter plot by setting x="price_change_percentage_24h" and y="price_change_percentage_7d". (4 points)
- Optimize the Clusters with Principal Component Analysis (10 points)
To receive all points, you must:
  - Create a PCA model instance, and set n_components=3. (1 point)
  - Use the PCA model to reduce the features to three principal components, then review the first five rows of the DataFrame. (2 points)
  - Get the explained variance to determine how much information can be attributed to each principal component. (2 points)
  - Answer the following question: What’s the total explained variance of the three principal components? (3 points)
  - Create a new DataFrame with the PCA data. Be sure to set the coin_id index from the original DataFrame as the index for the new DataFrame. Review the resulting DataFrame. (2 points)
- Find the Best Value for k by Using the PCA Data (10 points)
To receive all points, you must:
  - Code the elbow method algorithm, and use the PCA data to find the best value for k. Use a range from 1 to 11. (2 points)
  - Visually identify the optimal value for k by plotting a line chart of all the inertia values computed with the different values of k. (5 points)
  - Answer the following questions: What’s the best value for k when using the PCA data? Does it differ from the best value for k that you found by using the original data? (3 points)
- Cluster the Cryptocurrencies with K-Means by Using the PCA Data (10 points)
To receive all points, you must:
  - Initialize the K-means model with four clusters by using the best value for k. (1 point)
  - Fit the K-means model by using the PCA data. (1 point)
  - Predict the clusters for grouping the cryptocurrencies by using the PCA data. Review the resulting array of cluster values. (3 points)
  - Create a copy of the DataFrame with the PCA data, and then add a new column to store the predicted clusters. (1 point)
  - Using pandas’ plot, create a scatter plot by setting x="PC1" and y="PC2". (4 points)
- Determine the Weights of Each Feature on Each Principal Component (15 points)
To receive all points, you must:
  - Create a DataFrame that shows the weights of each feature (column) for each principal component by using the columns from the original scaled DataFrame as the index. (10 points)
  - Answer the following question: Which features have the strongest positive or negative influence on each component? (5 points)
- Coding Conventions and Formatting (10 points)
To receive all points, you must:
  - Place imports at the top of the file, just after any module comments and docstrings, and before module globals and constants. (3 points)
  - Name functions and variables with lowercase characters, with words separated by underscores. (2 points)
  - Follow DRY (Don't Repeat Yourself) principles, creating maintainable and reusable code. (3 points)
  - Use concise logic and creative engineering where possible. (2 points)
- Deployment and Submission (10 points)
To receive all points, you must:
  - Submit a link to a GitHub repository that’s cloned to your local machine and that contains your files. (4 points)
  - Use the command line to add your files to the repository. (3 points)
  - Include appropriate commit messages in your files. (3 points)
- Code Comments (10 points)
To receive all points, your code must:
- Be well commented with concise, relevant notes that other developers can understand. (10 points)

### Grade: 100
### Feedback from Grader:
Hey Geoff,



Great job on your Module 11 submission! You’ve clearly put a lot of effort into this assignment, and it shows in your technical skills, organization, and presentation.



First off, I appreciate how you’ve organized your code. Placing all imports at the top and following proper naming conventions for functions and variables makes your code easy to follow. Your comments are concise and relevant, helping to understand each step without getting lost.



You’ve done a fantastic job loading and normalizing the data. Using `StandardScaler()` to normalize the data was correctly implemented, and the resulting scaled DataFrame was handled well. Just make sure to always display and verify the scaled DataFrame to ensure everything is set up correctly.



Your implementation of the elbow method to find the best value for k is spot on. You created the list of k values, calculated the inertia for each, and plotted the elbow curve perfectly. Visually identifying the optimal k value is a crucial step, and you’ve done it well. Make sure to state this optimal value explicitly in your comments or markdown cells for clarity.



Clustering with K-Means using the original scaled data was handled very well. Initializing the model, fitting it, predicting clusters, and creating a scatter plot to visualize the clusters were all done correctly. The specific use of price change percentages for the axes in your scatter plot was a good choice.



Performing PCA and reducing the features to three principal components was another highlight. You correctly implemented the PCA, calculated the explained variance, and created a new DataFrame with the PCA data. It’s important to always clearly state the total explained variance for transparency.



Finding the best k value using PCA data was executed just as well as with the original data. The elbow method was applied correctly, and the optimal k value was identified and compared with the original data’s k value, which is excellent practice.



Your analysis using PCA data for clustering also stands out. Initializing and fitting the K-Means model, predicting clusters, and visualizing them with a scatter plot of principal components were done perfectly.



Creating a DataFrame to show the feature weights on each principal component was handled well, and identifying the features with the strongest influence was insightful. This part of the analysis is crucial for understanding the impact of each feature.



Your deployment and submission were seamless. The use of GitHub for version control and submitting the repository link shows your understanding of good coding practices. Just make sure your commit messages are descriptive and meaningful for better clarity.



Your code comments were another strong point. They were concise, relevant, and helpful for anyone reading your code.



Overall, you’ve done an exceptional job. Your technical skills, organization, and presentation are commendable. Keep up the excellent work, and continue to refine your attention to detail for even better results.



Best regards,



C.G - Learning Specialist
Central Grader , Jul 25, 2024 at 6:16am
