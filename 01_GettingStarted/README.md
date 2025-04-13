# Session 1: Getting Started

## What is Computational Thinking?

In this seminar, by *computational thinking* we mean a structured thinking and general problem solving process. (Which almost always involves some kind of computation, but the focus is on the sincire addressing of the problem and the honest interpretation of the results.)

For the model making processes we will usually use following [4 main steps](https://files.wolframcdn.com/pub/www.computerbasedmath.org/solution-helix-poster/cbm-helix-of-maths-poster-uk.pdf):

- Definition of the problem and asking relevant questions,
- Abstraction of the questions into computable format,
- Computation on data resulting various plots, charts, quantities, and finally,
- Interpret the results and see how well we addressed the original questions and how could we go further.

### Alternatives to computational thinking

Computational thinking is not "the only game in town" i.e. there are many other ways to think, set goals and address problems. Problem solving and navigating life is more of an Art then a systemizable process. However to mention a few alternatives to computational thinking see the following incomplete list:

- [Design Thinking](https://designthinkingmeite.web.unc.edu/wp-content/uploads/sites/22337/2020/02/Tim-Brown-Design-Thinking.pdf)
    - Usually a user/human centered itarative and collaborative process, gauging empathy to understand the needs and preferences of the users.
    - An essential part of any product or application development process.  
- [Systems Thinking](https://research.fit.edu/media/site-specific/researchfitedu/coast-climate-adaptation-library/climate-communications/psychology-amp-behavior/Meadows-2008.-Thinking-in-Systems.pdf)
    - A holistic approach focusing on the emergent properties of a system, which might be hard to compute precisely but some overall behaviour might be inferred.
    - It is often used in the context of complex systems, such as ecosystems, economies, and social systems.
- [Lateral Thinking](https://archive.org/details/seriouscreativity1992ocrgood/Serious-Creativity-1992-Ocr-Good/)
    - Creativity and unconventional approaches: Encourages shifting perspectives, defying logical constraints, and suspending assumptions.
    - An intuitive approach can suite well for choosing a problem and setting a – personal – goal.

(Here I will not mention Critical Thinking and Creative Thinking as alternatives because they are integrated in the flawour of Computational Thinking we will use in this seminar.)

However addressing real world problems is fundamentally an Art, and dogmatic systems are usually too rigid to address them adequately. The listed systemized approaches can be viewed as a set of tools which might be useful in some cases.

## Plan of the seminar

In the first sessions will be about computational and programming tools which can be used to complete the Final Project:
- Elements of the Open Source Software ecosystem:
    - GitHub, Git,
    - Python, virtual environments, IDEs
    - Jupyter notebooks
    - Google Colab
- Online coding and learning platforms 
    - LeetCode, 
    - W3Schools, 
    - Wolfram blogs (for project ideas and inspiration)
- Generative AI tools
    - ChatGPT, 
    - Claude, 
    - Gemini, 
    - GitHub Copilot

### Final Project

An essential and non-trivial part of the seminar is choosing a Final Project topic. Students have the freedom to propose their own projects based on their interests skills and future plans.

The final project has to contain at least one iteration of the listed four steps of the Computational Thinking process, containing:
- A clear description of the addressed problem,
- data collection and/or generation,
- computation and/or data analysis,
- and an honest interpretation of the results.

The Final Project will be a *Computational Essay* (preferably in a Jupyter notebook), accessible publicly on GitHub and/or Google Colab.
The best projects will be offered to develop to a technical blogpost and hopefully published in an online journal/blog series.

### Three Computational Essays

The second half of the seminar will be dedicated to give a menu containing various topics which can be addressed by computational thinking and show examples for Computational Essays.

The chosen topics will be:
- Mathematics & Synthetic data
    - Mathematical modelling, Monte Carlo integration
- Physical chemistry & modelling Real Data
    - Data modelling, linear and nonlinear fitting
- Computational Poetry & ML Basics
    - Machine learning, author guessing "AI"

### Final Project Presentations

The last session will be dedicated to the Final Project presentations. The students will present their projects in a 5-10 minutes long presentation. Peers and the seminar leader will review the projects and the best ones will be selected for further development and publication.

## Getting started with Git and GitHub

> Git is a tool useful primarely for developing and maintaining large collaborative software projects.

We will use only a tiny fraction of its capabilities, but GitHub will give a visibility to your project and familiarity with it will be helpful in the future.

A few Online tutorials:
- [Git Tutorial For Dummies](https://www.youtube.com/watch?v=mJ-qvsxPHpY)
- [How to create your first GitHub repository](https://www.youtube.com/watch?v=-RZ03WHqkaY)
- [Git Tutorial for Beginners](https://www.youtube.com/watch?v=8JJ101D3knE)

### Installing [Git](https://git-scm.com/)

Usually Linix and MacOS machines have Git preinstalled. To check if you have it, open a terminal and type:
```bash
$ git --version
```

If you see a version number, you have it installed. If not, you can install it using the package manager of your system.

For **Windows**, you can download the installer from the [Git website](https://git-scm.com/download/win) (or [Git for Windows](https://gitforwindows.org/) website) and follow the installation instructions.
- See a brief tutorial [here](https://www.youtube.com/watch?v=cweFdzKMeS0).

### Setting up Git locally

- Open a terminal (or Git Bash on Windows) and create and navigate to a project folder:
```bash
$ mkdir TestProject
$ cd TestProject
$ touch HelloWorld.ipynb
```

- Create a new Git repository:
```bash
$ git init
```

- make local setup:
```bash
$ git config --local user.name "Your Name"
$ git config --local user.email youremail
```
(This is editing the `.git/config` file in the current directory.)

- add the file to the repository:
```bash
$ git add .
```

- commit the changes:
```bash
$ git commit -m "Initial commit"
```

- check the status of the repository:
```bash
$ git status
```
### Creating a [GitHub](https://github.com/) repository

(GitHub has a few popular alternatives, such as [GitLab](https://gitlab.com/) and [Bitbucket](https://bitbucket.org/). We will use GitHub for this seminar because of its popularity, long history, big community and the large number of available resources.)

First you might need to [create a GitHub account](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github). (If you already have one, you can skip this step.)

- For creating a new account see [this tutorial](https://www.youtube.com/watch?v=h5cKAd94QNo).
    - You will need to have and verify your email address.
    - You will need to choose a username and password.
        - (Later you can [change your user name](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-user-account-settings/changing-your-github-username#changing-your-username) )

Assuming you have a GitHub account, you can create a new repository by following these steps:
- Log in to your GitHub account.
- Click on the "+" icon in the top right corner and select "New repository".
- Enter a name for your repository (e.g., "TestProject").
- Optionally, add a description.
- Choose the visibility of your repository (lets make it public for now).
- **Do not initialize this new repo with a README**—leave it empty (since you already have local files).
- Click on "Create repository".
- You will see a page with instructions on how to push your local repository to GitHub.

- Follow the instructions to push your local repository to GitHub:

### Connecting the Local and the Remote Repository

Firrst navigate to the local repository folder (if you are not already there) `$ cd TestProject`

As a good prectice check if the folder is not linked to any other remote repository:
```bash
$ git remote -v
```

Add the remote repository URL to your local repository:

```bash
$ git remote add origin https://github.com/NEW_GITHUB_USERNAME/TestProject.git
```

Create the main branch:

```bash
$ git branch -M main
```

Push the changes to GitHub:

```bash
$ git push -u origin main
```

- Check if the files are uploaded to GitHub by refreshing the page.

### Adding a README file

- You can add a README file to your repository by creating a new file called `README.md` (a [markdown](https://www.markdownguide.org/basic-syntax/) file) in the root of your project folder.

- You can use the following template for your README file:
```markdown
# Project Title (Test Project)
## Description
A brief description of your project. (First public project)
## Installation
Instructions for installing and running your project. (Leave it empty for now)
## Usage
Instructions for using your project. (Leave it empty for now)
## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
```

The following command line will create and write the README file:
```bash
$ echo -e "# Test Project \n## Description \nFirst public project \n## License \nThis project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details" > README.md
```

(Alternatively you can use any text editor to create the file. For example, you can use `nano` in the terminal, or any code editor like Visual Studio Code, etc.)

- Add it to the repository:
```bash
$ git add README.md
```
- Commit the changes:
```bash
$ git commit -m "Added README file"
```
- Push the changes to GitHub:
```bash
$ git push
```
- Check if the README file is uploaded to GitHub by refreshing the page.