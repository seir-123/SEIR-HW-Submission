## SEIR 0508

### Homework Submission via Github Pull Requests

For this class, you will be submitting in links to your completed homework to our Google Classroom, and working with Github through what are known as Pull Requests.

We use both Github and the Google Classroom on the off chance that something isn't working with either site, we'll have the other one to use as a reference. Our goal is to give you the credit for the work you've done, and we want to make sure you aren't overly stressed when a submission goes wrong on either of them. 


Making Pull Requests on Github can be a bit difficult at first as there are a few necessary steps, but by the end of this week, you should have the hang of it.

Lets use this Repo as practice together to make sure we have a step by step guide to get everything working

### Part One - Bringing Git to our Local Machine

1) Fork this repo. You should see "github.com/~your_username~/SEIR-HW-Submission" in your browser URL. If it says SEIR-0508 instead of "Your Username", you have not forked it correctly

2) In your GA/Unit1 directory, clone down this repo. Again, make sure the cloned link you've copied has Your Username in it, not SEIR-0508.

3) Make a change to something in the directory, you can do this by creating a new file - cd into this directory (SEIR-HW-Submission) and then enter

```
touch test.txt
``` 

in your command line. This will create a new blank .txt file.

Run a quick "ls" in your terminal window and you should see

```
Readme.md

test.txt
``` 

on your screen.

### Part Two - Pushing our Changes up to Github

Now that we've made a change, we can enter our 3 magic Git commands to add our files and commit them, and then push them up to our repo.


4) 
```
git add .
``` 

Which will add All of our files in this directory to the Git stack


5)
```
git commit -m "ready for submission"
```

Which will create a Git Commit with a message of "ready for submission". You can change that message to be whatever you'd like for whatever step you are on or task you are working on (We'll discuss this more later!)


Once you have your Git files added and committed, they are Staged and ready to be pushed up. We do this with the command

6)
```
git push origin /branch-name/
```
usually, but not always, your branch's name will be main. So for the sake of our submission right now, we want to enter

```
git push origin main
```

Git Push is the Command to run this step. Origin tells Git that we are working from our local computer. Main is the name of the branch we're working on. If you are on a different branch, you'll need to put the name of that branch in instead of main. This will come up in future hw assignments, and be crucial for your P3, which is a group project. So make sure to keep an eye on what your branch name is, or you will get a red error message!

Once your Git directory has been pushed up, go to the Github page and refresh your browser, you should see your new txt file uploaded "a few seconds ago" , with your commit message next to it.


Now that our files have been pushed to the git ecosystem, we can make our pull request. 

### Part Three - Making the Pull Request

7) On the nav bar of the Github page, select "Pull Requests", then click the big green button "New Pull Request"

You will see two grey blocks, one will say "main", which is what your changes are going to merge into, which the other should say "your-username/main", or whichever branch you are working on

Once you click the "Create Pull Request" button you'll be brought to a new screen where you can add in text

When working on a project, you will put a short description of what changes you've made and why you are making the pull request, ie "Styling Buttons", "Fixing up Login functionality", "Resizing Images", or anything else you'll be tasked to do.

For the sake of this class, we want to know
 - Who you are - Make sure you have your Name (NOT your Github username) at the top
 - Whether or not you have Completed the Assignment
 - Your Comfort Level with the assignment between 1-5
 - Any additonal questions you have


Once you add those in, hit the big green button to open the Pull Request. You should now see your name in a list in that Pull Requests tab. When we review your assignment and give you the credit, we will Close the Pull Request. If you recieve an email saying something like "Pull Request Closed" it means we have checked your HW off and you are good to go for the assignment!

### Important!

Each time you change a file in a Git folder, you are creating a new "Head"

DO NOT edit anything in your browser, only work on your files in the code editor. If you work on any files in the browser, you will create a new head. This means that you will NOT be able to run your Git Push commands.

If this happens there are two ways to solve the problem, one is elegant, one using brute force.

The elegant way is to run a number of Rebase commands - this can take a few hours to work, and truth be told, it may not always work.

The brute force way is to simply copy any important work we've done into a notepad or other file, delete our current Git folder, re-clone down what we have, paste our work back in, and then run our Add, Commit, and Push commands. Again, this is not the most elegant way of fixing the problem, but it will fix it - in about 90 seconds - so for the sake of this class, we'll mostly be pushing this method.

Once you begin working in the field, your company will have a designated team that works solely on fixing Git issues, and will have their own protocol on how to fix Rebase/Head issues (though, don't be surprised if they tell you to just delete and re-clone there too!)
