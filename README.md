# fast.ai course notes

## lesson 1

start with [lesson 1](https://course.fast.ai/lessons/lesson1.html)

create [crestle](https://www.crestle.ai) account. this gives you a gpu enabled jupyter environment (in the cloud)

alternatively use [paperspace]() takes somewhat longer to setup but the video claims that you get more compute for the buck.

### setup paperspace

to get some initial money, go and read this [forum thread](https://forums.fast.ai/t/paperspace-referral-link/9323). 
then click on gradient offering which provides a gradient-0 plan for $0/m

1. select "01. Base Container Paperspace + Fast.AI 0.7.x"
2. choose "Quadro P4000" machine (.52$/h)
3. click "Create Notebook" (or click twice if you get some error message)

after the notebook has been created you'll get your jupyter environment with your running machine. to open the notebook click on the link with the public ip provided (eg from the [notebooks overview](https://www.paperspace.com/console/notebooks).

open the terminal window and call the following commands:

```
git pull
conda env update
```

### start lesson1.ipynb

do the following steps (in the browser 

1. change to tab "files" and open (double click) folder "courses"
2. open "dl1"
3. double click on "lesson1.ipynb" (should show the notbook that starts with "Image classification with Convolutional Neural Networks")

run video and notebook in parallel (stopped at 30' https://course.fast.ai/lessons/lesson1.html)

from this repository upload data/singledouble.zip (pics of asw24, asg32) to "/notebooks/courses/dl1/data" and unzip the file

1. go to (train|valid)/(single|double) folders and delete .DS_Store
2. change PATH variable in step 4 in notebook (PATH = "../../../data/singledouble/")
3. add more epochs (change to learn.fit(0.01, 10))
4. re-run all commands 

from the training you should see something like the output below:

```
HBox(children=(IntProgress(value=0, description='Epoch', max=10), HTML(value='')))

epoch      trn_loss   val_loss   accuracy   
    0      0.742759   0.860284   0.416667  
    1      0.770471   0.786383   0.416667  
    2      0.734739   0.725046   0.5       
    3      0.710923   0.66923    0.583333  
    4      0.696546   0.622867   0.583333  
    5      0.619066   0.591822   0.666667  
    6      0.56554    0.567124   0.666667  
    7      0.516718   0.543661   0.666667  
    8      0.469392   0.52621    0.666667  
    9      0.434655   0.508873   0.666667  

[array([0.50887]), 0.6666666865348816]
```

and get some single/double seater glider classification

TODO continue [video](https://course.fast.ai/lessons/lesson1.html) at 30'
