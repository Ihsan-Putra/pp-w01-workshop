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
- Whenever you "accept an assignment" using the links on Learn, a repo is created for you online on GitHub.
- When you **clone** that repo onto your computer, you download the files in the GitHub repo. The changes you make to these files are *only* on your computer, until you *push* them back to the GitHub repo. We will go through that process today.

The team repository you created (by accepting the assignment and creating/joining your team) lives online for the moment, on GitHub.

### Driver, your instructions:

- First of all, in Zoom, share your screen with your teammate, so that they can see what you do.

- Then, if you haven't done this already, clone the GitHub repository on your computer using Atom. To do this:
1. Launch Atom.
2. If you followed the instructions to set up your system earlier this week, then in the pane on the left, you will see the last folder and files you were working on (probably `pp-w01-tutorial-<your github username>`). Right-click on the name of the folder, and select "Remove project folder". This doesn't delete anything, it just cleans up Atom so that you can start working on another project.
3. You should now see the "Clone an existing GitHub repository" button in the GitHub pane. Use it to clone the new GitHub repo, which should be called `pp-w01-workshop-<your team name>`.
4. You should now see these files in the left pane.

If you have encountered any issues so far, please call a tutor.

- In Atom, open the file `hello.py`. This is a **Python script**, which you can recognise with the extension `.py`. This can only contain Python code.

- You will see that there is already some code in there. Let's try to run it:

### 

## Notes

- If you can't decide who should be the driver first, pick the person who is currently closest to the North Pole.
- Throughout a pair programming session, the driver and the navigator should **communicate** as much as possible. For example, when typing code, the driver can explain what they want to do, talk through their thought process, ask the navigator for help; the navigator can provide feedback on the code, ask the driver to do something differently, spot mistakes and suggest corrections, consult the documentation (or other notes)...
- Today, you have used a shared GitHub repository to collaborate on a task. You also have GitHub repositories for your tutorial worksheets every week, which only belong to you -- you can still push your local changes to GitHub. It's a very good way to keep an online backup of your work -- in fact, this is how you will submit your projects later on.
