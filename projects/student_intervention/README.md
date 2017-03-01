# Project 2: Supervised Learning
## Building a Student Intervention System

You can go through the project by [Jupyter nbviewer](http://nbviewer.jupyter.org/github/daniellaah/Udacity-Machine-Learning-Projects/blob/master/projects/boston_housing/boston_housing.ipynb)

### Core Technique
1. Numpy Basic
2. Pandas Basic
4. Sklearn Basic
3. SVM, more about SVM see thses blogs:
  - [CS229机器学习笔记(五)-SVM之函数间隔, 几何间隔](http://daniellaah.github.io/2016/CS229-Machine-Learning-Notes-Lecture-6.html)
  - [CS229机器学习笔记(六)-SVM之拉格朗日对偶, 最优间隔分类器](http://daniellaah.github.io/2016/CS229-Machine-Learning-Notes-Lecture-7.html)
  - [CS229机器学习笔记(七)-SVM之Kernels](http://daniellaah.github.io/2016/CS229-Machine-Learning-Notes-Lecture-8.html)
  - [CS229机器学习笔记(七)-SVM之软间隔](http://daniellaah.github.io/2016/CS229-Machine-Learning-Notes-Lecture-8-1.html)
4. Hyper Parameter Tuning with Grid Search
5. to see more about Numpy, you can go to this repo:[Numpy, Pandas, Matplotlib学习笔记](https://github.com/daniellaah/python-scientific-computing)

### Install

This project requires **Python 2.7** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [scikit-learn](http://scikit-learn.org/stable/)

You will also need to have software installed to run and execute an [iPython Notebook](http://ipython.org/notebook.html)

Udacity recommends our students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 

### Code

Template code is provided in the notebook `student_intervention.ipynb` notebook file. While some code has already been implemented to get you started, you will need to implement additional functionality when requested to successfully complete the project.

### Run

In a terminal or command window, navigate to the top-level project directory `student_intervention/` (that contains this README) and run one of the following commands:

```ipython notebook student_intervention.ipynb```  
```jupyter notebook student_intervention.ipynb```

This will open the iPython Notebook software and project file in your browser.

## Data

The dataset used in this project is included as `student-data.csv`. This dataset has the following attributes:

- `school` : student's school (binary: "GP" or "MS")
- `sex` : student's sex (binary: "F" - female or "M" - male)
- `age` : student's age (numeric: from 15 to 22)
- `address` : student's home address type (binary: "U" - urban or "R" - rural)
- `famsize` : family size (binary: "LE3" - less or equal to 3 or "GT3" - greater than 3)
- `Pstatus` : parent's cohabitation status (binary: "T" - living together or "A" - apart)
- `Medu` : mother's education (numeric: 0 - none,  1 - primary education (4th grade), 2 - 5th to 9th grade, 3 - secondary education or 4 - higher education)
- `Fedu` : father's education (numeric: 0 - none,  1 - primary education (4th grade), 2 - 5th to 9th grade, 3 - secondary education or 4 - higher education)
- `Mjob` : mother's job (nominal: "teacher", "health" care related, civil "services" (e.g. administrative or police), "at_home" or "other")
- `Fjob` : father's job (nominal: "teacher", "health" care related, civil "services" (e.g. administrative or police), "at_home" or "other")
- `reason` : reason to choose this school (nominal: close to "home", school "reputation", "course" preference or "other")
- `guardian` : student's guardian (nominal: "mother", "father" or "other")
- `traveltime` : home to school travel time (numeric: 1 - <15 min., 2 - 15 to 30 min., 3 - 30 min. to 1 hour, or 4 - >1 hour)
- `studytime` : weekly study time (numeric: 1 - <2 hours, 2 - 2 to 5 hours, 3 - 5 to 10 hours, or 4 - >10 hours)
- `failures` : number of past class failures (numeric: n if 1<=n<3, else 4)
- `schoolsup` : extra educational support (binary: yes or no)
- `famsup` : family educational support (binary: yes or no)
- `paid` : extra paid classes within the course subject (Math or Portuguese) (binary: yes or no)
- `activities` : extra-curricular activities (binary: yes or no)
- `nursery` : attended nursery school (binary: yes or no)
- `higher` : wants to take higher education (binary: yes or no)
- `internet` : Internet access at home (binary: yes or no)
- `romantic` : with a romantic relationship (binary: yes or no)
- `famrel` : quality of family relationships (numeric: from 1 - very bad to 5 - excellent)
- `freetime` : free time after school (numeric: from 1 - very low to 5 - very high)
- `goout` : going out with friends (numeric: from 1 - very low to 5 - very high)
- `Dalc` : workday alcohol consumption (numeric: from 1 - very low to 5 - very high)
- `Walc` : weekend alcohol consumption (numeric: from 1 - very low to 5 - very high)
- `health` : current health status (numeric: from 1 - very bad to 5 - very good)
- `absences` : number of school absences (numeric: from 0 to 93)
- `passed` : did the student pass the final exam (binary: yes or no)


Ada boost:
This is an excellent paper by Rob Schapire, one of the creators of Adaboost from Stanford. You may have a look in your spare time - http://rob.schapire.net/papers/explaining-adaboost.pdf

Another excellent technical one paper is this one - http://math.mit.edu/~rothvoss/18.304.3PM/Presentations/1-Eric-Boosting304FinalRpdf.pdf

This one is very nice for intuitive understanding - http://machinelearningmastery.com/boosting-and-adaboost-for-machine-learning/

KNN:
A simplified explanation of KNN could be found here - https://www.analyticsvidhya.com/blog/2014/10/introduction-k-neighbours-algorithm-clustering/

This one is a very short description, but nice one - http://www.saedsayad.com/k_nearest_neighbors.htm

Some more KNN slides for you - http://www.csee.umbc.edu/~tinoosh/cmpe650/slides/K_Nearest_Neighbor_Algorithm.pdf

SVM:
Here is a tutorial on SVM by Jason Weston, a very famous Machine Learning Researcher now working at Facebook - http://www.cs.columbia.edu/~kathy/cs4701/documents/jason_svm_tutorial.pdf

This last one is just as it’s name implies - An Idiot’s Guide to Support Vector Machines.
http://svms.org/tutorials/Berwick2003.pdf
