# Udacity Data Science Nanodegree
# Project 06: Recommendations with IBM

--------------------------------------
1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## 1. Installation <a name="installation"></a>

- This code was created by using Python versions 3.*.
- Following libraries are required:

* pandas
* numpy
* matplotlib
* pickle

- To answer the questions within the notebook, you have to import the *project_test* module
- copy repository: git clone https://github.com/oliverkroening/Udacity_DSND_Project06


## 2. Project Motivation <a name="motivation"></a>
In this project, I will put the recommendation skills, I got in the current Udacity lessons, to use on real data.

The dataset, I will work with in this project, contains interactions between user of a platform and articles. The aim of my work is to perform several recommendation techniques on this data. Therefor, I will use rank-based recommendations, user-based collaborative filtering and matrix factorizations to find recommended articles for certain users.

## 3. File Descriptions <a name="files"></a>  
The project mainly consists of a jupyter notebook:
- `Recommendations_with_IBM.ipynb` 

The data can be found in the `data` folder and consists of
- `articles_community.csv` (article descriptions) 
- `user-item-interactions.csv`(interactions of users, indicated by hashed e-mail, and articles, indicated by article IDs and titles)

Following files are used to answer the questions within the notebook:
- `project_test.py`(module with functions to check the right answers)
- `top_20.p`(checks top 20 articles)
- `top_10.p`(checks top 10 articles)
- `top_5.p`(checks top 5 articles)

Furthermore, I included the submitted and reviewed HTML-file that contains the jupyter notebook.

## 4. Results <a name="results"></a>
Three recommendation techniques are shown in this project:

- Rank-based recommendations:
The functions return the most common and most frequently interacted articles for the user

- User-user based collaborative filtering:
A user-item-matrix is created and similar users are identified. According to the articles the similar users have interacted with, the functions will recommend sorted articles for a certain user ID.

- Matrix Factorization:
To reproduce the user-item matrix, I performed a Singular Value Decomposition (SVD) on the matrix. The obtained matrices U, S, Vt are then examined to find a reasonable number of latent factors. After creating training and test datasets and training the model, I visualize the influence of the number of latent factors on the matrix to prevend overfitting.

## 5. Licensing, Authors, Acknowledgements<a name="licensing"></a>
All data was provided by Udacity, thus, I must give credit to them. Other references are cited in the Jupyter notebook.
Please refer to [Udacity Terms of Service](https://www.udacity.com/legal) for further information.
