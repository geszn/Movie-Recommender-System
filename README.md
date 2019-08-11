## Movie Recommendation System with Matrix Factorization and Hyperparameter tuning

Recommendation system is developed to match consumers with product to meet their variety of special needs and tastes in order to enhance user satisfaction and loyalty. The popularity of personalized recommendation system has been increased in recent years and applied in several areas include movies, songs, books, news, friends recommendations on social media, travel products, and other products in general. This repo shows a set of Jupyter Notebooks demonstrating a variety of movie recommendation systems for the MovieLens 100K dataset. It consists of 90,570 ratings from 943 users on 1682 different movies.

Used:
* Matrix Factorization with Hyperparameter tuning to recommend movies by Matrix decompositions.
* Root Mean Square Error (RMSE) to measure similarity between two users.

## Requirements
* Python 2.7
* Jupyter Notebook

## Dependencies
* Pandas
* GraphLab

## Install Dependencies
### Step 1 : Install virtual environment
Setting execution policy to unrestricted is essential to enable running of script in powershell
```
Get-ExecutionPolicy
Set-ExecutionPolicy unrestrictedpip install virtualenv
cd ~targetlocation
virtualenv gl-env
gl-env/Scripts/activate
```

### Step 2 : Install Jupyter Notebook
Install it inside virtual environment gl-env
```
# Install IPython Notebook (optional)
pip install "ipython[notebook]"
```

### Step 3 : Install GraphLab Create
Install this also inside virtual environment gl-env
```
# Install your licensed copy of GraphLab Create
pip install --upgrade --no-cache-dir https://get.graphlab.com/GraphLab-Create/2.1/your registered email address here/your product key here/GraphLab-Create-License.tar.gz
```

### Step 4 : Check if installed
Simply type python in the gl-env to activate python terminal
```
python
>>>import graphlab
```
If you get the following error:
```
ACTION REQUIRED: Dependencies libstdc++-6.dll and libgcc_s_seh-1.dll not found.1. Ensure user account has write permission to C:\Users\Bee\Desktop\Coursera\gl-env\lib\site-packages\graphlab
2. Run graphlab.get_dependencies() to download and install them.
3. Restart Python and import graphlab again.By running the above function, you agree to the following licenses.* libstdc++: https://gcc.gnu.org/onlinedocs/libstdc++/manual/license.html
* xz: http://git.tukaani.org/?p=xz.git;a=blob;f=COPYING
```
simply run it in python terminal
```
graphlab.get_dependencies()
```
And then import again and it should work.

## Output
Top 5 movie recommendations for 5 users using Matrix Factorization method with Regularization hyperparameter = 1e - 5
![item1](https://user-images.githubusercontent.com/14583471/62832620-b5d61080-bc63-11e9-8a89-767e8ca6ceec.jpg)

RMSE comparison
![item2](https://user-images.githubusercontent.com/14583471/62832626-d8682980-bc63-11e9-8a79-670f7be802b1.jpg)

Evaluation of processing time
![Item3](https://user-images.githubusercontent.com/14583471/62832627-db631a00-bc63-11e9-8daa-e8dda1d936e8.jpg)
