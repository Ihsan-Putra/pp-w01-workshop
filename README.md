# Week 1 workshop - Pair-programming

In most workshops in this course, you will work on a programming task together with a partner, using a method called **pair programming**. This week's task is designed for you to try it out, and to become familiar with the workflow.

## What is pair programming?

Pair programming is a method where two people (usually) sit in front of the same computer. Each person has a specific role:
- The **driver** writes and runs the code, and is the only person allowed to do it. They explain what they do to the navigator.
- The **navigator** observes and helps the driver, spots errors in the code, gives suggestions and ideas... They are not allowed to write code.

The two programmers decide who should "drive" first, and that person takes the keyboard to start working. The other person, the navigator, watches the screen and helps the driver with the task -- without touching the mouse or keyboard.

Then, after a while, the driver passes the keyboard and mouse to the navigator, and they switch roles.

## How does it work online?

This year, unfortunately, you won't be able to sit next to your partner and to share a computer. Instead, you will use Zoom to communicate and share your screens, and GitHub to "pass the keyboard" when you switch roles.

The task this week contains detailed instructions about what to do and when, so you can have a better idea of how this works in practice. There will be less and less scaffolding in future workshops -- it will feel more natural after you've done it a few times. During workshops, we will typically ask you to switch roles every 15 minutes or so, to make sure that both you and your partner take both roles at least once.

## Instructions

First, decide who should be the "driver" first (you will switch roles later).

### Create your team repository on GitHub

If you made it here (following the instructions on Learn), then you probably have done this already -- congratulations! Both you and your partner are now **contributors** to the *same* GitHub repository -- you can both change the code in the repo.

A quick note:
- a **repository** is basically just a folder with some files inside, generally managed with git.
- a **repo** is just short for "repository".
- a **local repo** is a repository located on your computer (not online).
- Whenever you "accept an assignment" using the links on Learn, a repo is created for you online on GitHub.
- When you **clone** that repo onto your computer, you download the files from the GitHub repo, and you also create a "link" (called a *remote*) from your local repo to the GitHub repo. The changes you make to these files are *only* on your computer, until you *push* them back to the GitHub repo. We will go through that process today.

The team repository you created (by accepting the assignment and creating/joining your team) lives online for the moment, on GitHub.

### Let's start coding!

- **Driver:** first of all, in Zoom, share your screen with your teammate, so that they can see what you do. When you code something, explain what you are doing out loud.
- **Navigator**: help the driver by reading these instructions to them, so they don't have to keep coming back here to read them all the time.

#### Driver:

- If you haven't done this already, clone the GitHub repository on your computer using Atom. To do this:
1. Launch Atom.
2. If you followed the instructions to set up your system earlier this week, then in the pane on the left, you will see the last folder and files you were working on (probably `pp-w01-tutorial-<your github username>`). Right-click on the name of the folder, and select "Remove project folder". This doesn't delete anything, it just cleans up Atom so that you can start working on another project.
3. You should now see the "Clone an existing GitHub repository" button in the GitHub pane. Use it to clone the new GitHub repo, which should be called `pp-w01-workshop-<your team name>`. If you don't remember how to do this, you can ask your **navigator** for help.
4. You should now see these files in the left pane. Note that these instructions here are in the file `README.md`.

*If you have encountered any issues so far, please call a tutor.*

- In Atom, open the file `hello.py`. This is a **Python script**, which you can recognise with the extension `.py`. This can only contain Python code.

- You will see that there is already some code in there. Let's try to run it: in Atom, select all 4 lines (with your mouse), and press Ctrl+Enter (Windows, Linux) or Cmd+Enter (MacOS) to run the code (just like in Jupyter). You should see the *output* of the code appear next to line 4.

*If this doesn't work, please call a tutor.*

#### Driver & navigator:

Discuss together to figure out how the `print()` command works here. Driver, you can try to remove the `f` in front of the quote `'`, and run the code again to see what happens; you can also try changing what's inside the `{}`. Navigator, you can consult the documentation [here](https://docs.python.org/3/tutorial/inputoutput.html#formatted-string-literals) and explain it to your driver.

#### Driver:

- On lines 1 and 2, change the variables `name` and `age` to reflect your own name and age.

- On line 3, create a new variable called `birthday`, a *string* which indicates when is your birthday. For example, if your birthday is this Sunday, `birthday` could be `'27th September'`.

- Then, after the `print()` command, add another line to print a sentence which says when is your birthday. Run all the code again, and check that it worked. If it doesn't work, ask your navigator to help you find the error.

Now, you are going to save your changes using git, and update the GitHub repo with your new code. There will be 3 steps to this process:
1. You need to first tell git that you've changed some files. This is called **staging** your changes.
2. Then, you will tell git to **commit** these changes, i.e. to save them in your local repo.
3. Finally, you will tell git to **push** the changes online to the GitHub repo, so that your collaborator can also see them.

This is what you need to do:

- Press Ctrl+s (Windows, Linux) or Cmd+s (MacOS) to save the file.

- Then, click on the "Git" button in the bottom right in Atom, to open the Git pane. You should see that the file `hello.py` appears in a section called "Unstaged changes". Click "Stage All" to stage your changes -- now, git knows about them, and the file `hello.py` should have moved to the section called "Staged changes".

- Now, you are going to commit these changes. **Whenever you commit**, you should write a **short message** to describe what changes you've made. Type a message in the text box called "Commit message"; for example, your message could be "Added my birthday to hello.py". Then, click "Commit to master".

Your changes have now been committed to your *local* repo.

#### Navigator:

Go to the repo on GitHub, refresh the page, and check the file `hello.py` -- you should see that it hasn't changed yet.

#### Driver:

The final step is for you to **push** these files from your computer to GitHub. Click the "Push" button at the bottom of the Git pane in Atom to do this, and wait a few seconds for this to finish.

#### Navigator:

Refresh the page again, and check `hello.py` -- you should now see the changes.

### Time to switch roles!

Navigator, you are now the **driver**, and vice versa.

- **(New) driver**: on Zoom, share your screen. You might need to ask your navigator (the former driver) to stop sharing their screen first. Explain what you do out loud for your navigator to follow more easily.
- **(New) navigator**: you are now in charge of reading the instructions for your driver, observing what they do, and helping them when necessary.

#### Driver:

Go back to the GitHub repo, which is now updated with the latest changes.

- If you had already cloned the repo on your computer before starting the exercise, then go to Atom, open the Git pane, and click "Fetch", which will download the latest changes from GitHub. Click "Pull" to update your local repo with these changes.
- If you have not cloned the repo yet, go back to the first "Driver:" section, and follow the same instructions to clone it.

You should now see the files in Atom, including the changes that the previous driver just made. If you've had any issues with this, please call a tutor.

- Open `hello.py` and run the code yourself (select it, and press Ctrl+Enter or Cmd+Enter) to check that it still works. (It should!)

- Change the values of `name`, `age`, and `birthday` to your own name, age, and birthday.

- Delete the line that prints when your birthday is.

- Write a new line to print a sentence which says that you will be one year older on your birthday. For instance, with the example values that were in the code at the beginning of the workshop, that could be something like:

> On the 27th October, I will be 37 years old.

The date and age should correspond to your own, and you are not allowed to type them or copy/paste them explicitly into the `print()` command. Run the code and check that it works.

#### Navigator:

Help your driver figure out how to do this. You can also look at the documentation [here](https://docs.python.org/3/tutorial/inputoutput.html#formatted-string-literals). If the code doesn't work the first time, help the driver to find the error.

#### Driver:

Save the file, stage your changes, commit them, and push them to GitHub. You can ask your navigator to read you the instructions again from the previous section.

#### Navigator:

After the changes have been pushed, refresh the GitHub repo to check that this has worked -- you should see the new code there. Then, go back to Atom, click "Fetch" and then "Pull" in the Git pane, and check that you now also have the changes in your local `hello.py` file.

## Victory!

Well done -- you now know how to pair-program, how to use git to manage your changes, and how to work collaboratively on a shared GitHub repository.

If you still have time before the end of the workshop, then please continue working like this together. You can change roles again now (don't forget to change who shares their screen), and continue adding and changing things to the code, if you want to get more practice with git. **Don't forget to stage and commit your changes regularly**, even if you are not switching roles immediately! Also, **don't forget to switch roles** at least a couple more times.

Here are some suggestions:

- Instead of changing the values of `name`, `age`, and `birthday`, change the variable names to e.g. `name_1`, `age_1`, and `birthday_1`, and add 3 new variables `name_2`, `age_2`, and `birthday_2`, so that both your names, ages, and birthdays are kept in memory. Add another command to print that information for both of you.

- Using **comparison operators** (you can't type 'True' or 'False' yourself), try to print the following:

> Is <person 1> younger than <person 2>? <True/False>

where <person 1> and <person 2> are your respective names, and <True/False> is either `True` or `False` (the Boolean value) depending on your ages. Again, no typing names or ages in the `print()` command!

- Create more variables to print information about yourselves to get to know each other a little better: where you are from, where you are currently located and what time it is there, what courses you are taking this semester... It's a bit like having a conversation using exclusively `print()` commands.

- You can also create a new Python script: right-click anywhere in the left pane in Atom, select "New File", and give it a name -- don't forget the `.py` extension. Write some code in it, run it; stage, commit, and push your changes for that new file to appear in the GitHub repo. You could create a new script like this to work together on one of the tutorial worksheet problems, for example.

## Useful tips

- If you can't decide who should be the driver first, pick the person who is currently closest to the North Pole.
- Throughout a pair programming session, the driver and the navigator should **communicate** as much as possible. For example, when typing code, the driver can explain what they want to do, talk through their thought process, ask the navigator for help; the navigator can provide feedback on the code, ask the driver to do something differently, spot mistakes and suggest corrections, consult the documentation (or other notes)...
- Today, you have used a shared GitHub repository to collaborate on a task. You also have GitHub repositories for your tutorial worksheets every week, which only belong to you -- you can still push your local changes to GitHub. It's a very good way to keep an online backup of your work -- in fact, this is how you will submit your projects later on.
- If you want to go back to work on another local repo later, in Atom, click "File", select "Add Project Folder", and select the folder where that repo is located.
