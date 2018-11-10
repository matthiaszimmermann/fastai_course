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
