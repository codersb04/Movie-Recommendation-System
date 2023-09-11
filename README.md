# Movie-Recommendation-System
## Task:
Build a system for Movie Recommendation</br>
Used **Cosine Similarity**</br>
Tool Used: Jupyter Notebook, Python

## Dataset: 
Taken small dataset with 4803 records and 24 features:
- index                
- budget                
- genres              
- homepage            
- id                  
- keywords              
- original_language    
- original_title        
- overview            
- popularity        
- production_companies  
- production_countries  
- release_date          
- revenue            
- runtime           
- spoken_languages    
- status             
- tagline               
- title               
- vote_average         
- vote_count          
- cast                 
- crew                 
- director       </br></br>

Source: https://drive.google.com/file/d/1cCkwiVv4mgfl20ntgY3n4yApcWqqZQe6/view

## Working:
### Movie Recommendation System types:
- Content Based Recommendation System
- Popularity Based Recommendation System
- Collaborative Recommndation System
### Import Dependencies:
Libraries needed for the task:

- NumPy
- Pandas
- Difflib
- TfidfVectorizer
- Cosine Similarity
### Data Collection and Analysis:
- Load the CSV file and convert it to Pandas dataframe using read_csv function
- Analyse the data using function head, info, usnull and shape.
### Data Preprocessing:
- Select the necessary features needed for recommendation from the list of 24 features
- Handling the missing value: Replace the null value with the NULL string
- Convert the Text dat to Feature vector using TFifVectorizer
### Cosine Similarity:
- Apply the cosine similarity function
- Get the similarity score of each of 4809 records with each other, resulting the 2d array of shape (4809,4809)
### Build the System:
- Get the movie name from User
- Create list of all the movie title given in the dataset
- Find the closest match of movie name given by user to the movie list and get the first value from the matching movie name list
- Get the index of the most matched movie name
- Get the similarity score of the most matched movie with rest of the list along with the index value
- Sort the similarity list in desending order such that movie with high similarity would be at the top and the least score would be at the bottom
- Get the title of the movie using the index value and print the top 20 most matches according to there similarity score.
### Build a predictive system
- Combine all the code of the system built together and print the result</br></br></br>

Reference: Project 18. Movie Recommendation System using Machine Learning with Python, Siddhardhan, https://www.youtube.com/watch?v=7rEagFH9tQg&list=PLfFghEzKVmjvuSA67LszN1dZ-Dd_pkus6&index=18
