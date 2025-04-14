# Session 1: Getting Started

## What is Computational Thinking?

In this seminar, by *computational thinking* we mean a structured thinking and general problem solving process. (Which almost always involves some kind of computation, but the focus is on the sincere addressing of the problem and the honest interpretation of the results.)

For the model making processes we will usually use following [4 main steps](https://files.wolframcdn.com/pub/www.computerbasedmath.org/solution-helix-poster/cbm-helix-of-maths-poster-uk.pdf):

- Definition of the problem and asking relevant questions,
- Abstraction of the questions into computable format,
- Computation on data resulting various plots, charts, quantities, and finally,
- Interpret the results and see how well we addressed the original questions and how could we go further.

### Alternatives to computational thinking

Computational thinking is not "the only game in town" i.e. there are many other ways to think, set goals and address problems. Problem solving and navigating life is more of an Art than a systemizable process. However to mention a few alternatives to computational thinking see the following incomplete list:

- [Design Thinking](https://designthinkingmeite.web.unc.edu/wp-content/uploads/sites/22337/2020/02/Tim-Brown-Design-Thinking.pdf)
    - Usually a user/human centered iterative and collaborative process, using empathy to understand the needs and preferences of the users.
    - An essential part of any product or application development process.  
- [Systems Thinking](https://research.fit.edu/media/site-specific/researchfitedu/coast-climate-adaptation-library/climate-communications/psychology-amp-behavior/Meadows-2008.-Thinking-in-Systems.pdf)
    - A holistic approach focusing on the emergent properties of a system, which might be hard to compute precisely but some overall behaviour might be inferred.
    - It is often used in the context of complex systems, such as ecosystems, economies, and social systems.
- [Lateral Thinking](https://archive.org/details/seriouscreativity1992ocrgood/Serious-Creativity-1992-Ocr-Good/)
    - Creativity and unconventional approaches: Encourages shifting perspectives, defying logical constraints, and suspending assumptions.
    - An intuitive approach can suit well for choosing a problem and setting a – personal – goal.

(Here I will not mention Critical Thinking and Creative Thinking as alternatives because they are integrated in the flavour of Computational Thinking we will use in this seminar.)

However addressing real world problems is fundamentally an Art, and dogmatic systems are usually too rigid to address them adequately. The listed systemized approaches can be viewed as a set of tools which might be useful in some cases.

## Plan of the seminar

In the first sessions we will set up the computational and programming tools which can be used to complete the Final Project:
- Elements of the Open Source Software ecosystem:
    - GitHub, Git,
    - Python, virtual environments, IDEs
    - Jupyter notebooks
- Online coding and learning platforms
    - Google Colab, 
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

The second half of the seminar will be dedicated to giving a menu containing various topics which can be addressed by computational thinking and show examples for Computational Essays.

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

> Git is a version control tool, useful primarily for developing and maintaining large collaborative software projects.

We will use only a tiny fraction of its capabilities, but GitHub will give a visibility to your project and familiarity with it will be helpful in the future.

A few Online tutorials:
- [Git Tutorial For Dummies](https://www.youtube.com/watch?v=mJ-qvsxPHpY)
- [How to create your first GitHub repository](https://www.youtube.com/watch?v=-RZ03WHqkaY)

### Installing [Git](https://git-scm.com/)

Usually Linux and MacOS machines have Git preinstalled. To check if you have it, open a terminal and type:
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
- Choose the visibility of your repository (let's make it Public).
- **Do not initialize this new repo with a README**—leave it empty (since you already have local files).
- Leave the `.gitignore` on None (you can add it later).
- Leave the license on None (you can add it later).
- Click on "Create repository".
- You might see a page with instructions on how to push your local repository to GitHub.
  - "…or push an existing repository from the command line":
  - `git remote add origin https://github.com/GITHUB_USERNAME/TestProject.git`
  - `git branch -M main`
  - `git push -u origin main`

### Connecting the Local and the Remote Repository

First navigate to the local repository folder (if you are not already there) `$ cd TestProject`

As a good practice check if the folder is not linked to any other remote repository:
```bash
$ git remote -v
```

Add the remote repository URL to your local repository:

```bash
$ git remote add origin https://github.com/GITHUB_USERNAME/TestProject.git
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
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details (Will be added later)
```

The following command line will create and write the README file:
```bash
$ echo -e "# Test Project \n## Description \nFirst public project" > README.md
```

(Alternatively you can use any text editor to create the file. For example, you can use `nano` in the terminal, or any code editor like Visual Studio Code, etc.)

- Add it to the repository:
```bash
$ git add README.md
```
- Commit the changes:
```bash
$ git commit -a -m "Added README file"
```
- Push the changes to GitHub:
```bash
$ git push
```
- Check if the README file is uploaded to GitHub by refreshing the page.

#### Troubleshooting with password

If you have trouble with the password, you can use a [personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) instead of your password. You can create a personal access token in your GitHub account settings and use it as your password when pushing to GitHub.

**Prepare a text file to save your Token.** You might see it only once, so save it in a secure place. (You can use a password manager or a text file.)

[Generating a Classical token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#creating-a-personal-access-token-classic):
- Go to your GitHub account Settings. (Top Right corner, click on your profile picture, then click on "Settings").
- Click on "Developer settings" in the left sidebar (Bottom of the list).
- Click on "Personal access tokens" in the left sidebar.
- Click on "Tokens (classic)".
- Click on "Generate new token (classic)".
  - Select the expiration date (e.g. 90 days). (you could choose "No expiration" but it's not recommended for security reasons)
  - Select the scopes you want to grant it (for pushing to GitHub, you need the `repo` scope).
- Click on "Generate token".
- Copy the token and save it in a secure place (you won't be able to see it again).
- Use the token as your password when pushing to GitHub.

### Additional resources

- [GIT CHEAT SHEET](https://education.github.com/git-cheat-sheet-education.pdf)
- [Git Tutorial for Beginners](https://www.youtube.com/watch?v=8JJ101D3knE)
- [ProGit](https://git-scm.com/book/en/v2) book

## Virtual environments

Virtual environments are a way to create isolated Python environments for your projects. This allows you to manage dependencies and avoid conflicts between different projects.

### Creating a virtual environment

In this Seminar I suggest to use [Anaconda](https://www.anaconda.com/) for creating virtual environments. It is a popular distribution of Python for scientific computing and data science. It comes with a package manager called `conda` which makes it easy to create and manage virtual environments.
(You can also use `venv`, which is more light weight but it will be not covered here. If you are interested in it, you can find a tutorial [here](https://realpython.com/python-virtual-environments-a-primer/).)

### Installing Anaconda

- Download the Anaconda installer from the [Anaconda website](https://www.anaconda.com/download/success).
- Follow the installation instructions for your operating system.
- After installation, open a terminal (or Anaconda Prompt on Windows) and type:
```bash
$ conda --version
```

### Setting up a virtual environment

- Open a terminal (or Anaconda Prompt on Windows) and create a new virtual environment:
```bash
$ conda create --name testenv python=3.10
```

### Activating the virtual environment

- Activate the virtual environment:
```bash
$ conda activate testenv
```
- verify the activation:
```bash
$ conda info --envs
```
- check the Python version:
```bash
$ python --version
```

### Deactivating the virtual environment

- Deactivate the virtual environment:
```bash
$ conda deactivate
```

### Additional resources

- [Conda Cheat Sheet](https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf)


## IDE, Visual Studio Code

### Installing Visual Studio Code
- Download the installer from the [Visual Studio Code website](https://code.visualstudio.com/download).
- Follow the installation instructions for your operating system.
- After installation, open Visual Studio Code and install the Python extension:
    - Click on the Extensions icon in the left sidebar (or press `Ctrl+Shift+X`).
    - Search for "Python" and click on "Install" for the official Python extension by Microsoft.
- Install the Jupyter extension:
    - Search for "Jupyter" and click on "Install" for the official Jupyter extension by Microsoft.

## Hello World in Jupyter Notebook

- Create a New File in Visual Studio Code:
    - Click on the File menu and select "New File..." .
    - Select "Jupyter Notebook" from the list of file types.
    - To Set the kernel, click on the "Select Kernel" button in the top right corner and select the Python interpreter from your virtual environment. (e.g. `testenv`).
      - (you might need to install ipykernel in VS Code)
    - Write the following code in the first cell:
```python
print('Hello World')
```

- Run the cell by pressing `Shift+Enter`.
- Save the file as `HelloWorld.ipynb` in your project folder.

### Push the Hello World notebook to GitHub

Commit the changes:
```bash
$ git commit -a -m "Added Hello World notebook"
```
- Push the changes to GitHub:
```bash
$ git push
```
- Check if the notebook is uploaded to GitHub by refreshing the page.

## Congratulations

You have successfully created a GitHub repository, set up a virtual environment, and created a Jupyter notebook with a "Hello World" program.

**Great job!**