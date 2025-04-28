# Session 2: Tools, Resources & Complexity

## Online Resources

### Google Colab

- [Google Colab](https://colab.research.google.com/) - A free Jupyter notebook environment that runs in the cloud and stores notebooks on Google Drive.
Great for projects which does not require a lot of data and computational resources.
- Useful example notebooks:
   - [Markdown guide](https://colab.research.google.com/notebooks/markdown_guide.ipynb) - A guide to using Markdown in Colab notebooks.
   - [Overview of Colaboratory Features](https://colab.research.google.com/notebooks/basic_features_overview.ipynb) - An overview of the features available in Colab.
   - [External data: Local Files, Drive, Sheets, and Cloud Storage](https://colab.research.google.com/notebooks/io.ipynb) - A guide to using external data sources in Colab.
        - It seams that you need to give permission for all categories of data sources to use the IO methods shown in the notebook.
        - Default file write example `foo.txt` will appear in our "My Drive" folder in Google Drive.
    - [Gemini Snippets](https://colab.research.google.com/notebooks/snippets/gemini.ipynb) - A guide to using Gemini snippets in Colab.
       - You will need to generata an API key in Google AI Studio and set it in the notebook "Secrets".

    - [Google Earth Engine](https://colab.research.google.com/github/google/earthengine-community/blob/master/guides/linked/ee-api-colab-setup.ipynb) - A guide to using Google Earth Engine in Colab.
        - You might register the Google Earrth Engine project
        - You need to change 'my-project' in `ee.Initialize(project='my-project')` to your 'Project ID' for the Google EE project (accessible at [Google Cloud Console](https://console.cloud.google.com/))
        - See [Earth Engine Data Catalog](https://developers.google.com/earth-engine/datasets) for the list of datasets available in Google Earth Engine.

    - [Statistical Games](https://colab.research.google.com/drive/1dFSqVPMd0_6Ai8iMfoohOETQjdy2C2GD) recreates plots for a scientific paper, using the costum made [statgames](https://github.com/Konczer/UncertaintyTheory/tree/main/StatisticalGames/Software/Python/statgames) package.

    - Advanced materials in the [Eastern European Machine Learning](https://github.com/eemlcommunity) summer school resource page. (See colab Tutorials)

## Online learning resources

- [W3School](https://www.w3schools.com/) - A web development tutorial site. It has a lot of tutorials on HTML, CSS, JavaScript, Python, SQL, and more.
  - [W3School Python](https://www.w3schools.com/python/) - A tutorial on Python programming. It covers the basics of Python, including data types, variables, operators, loops, functions, and more.

- [Codeacadamy](https://www.codecademy.com/) - An interactive learning platform that offers free coding classes in various programming languages, including Python, Java, and C++.
  - [Intro to Data Visualization with Python](https://www.codecademy.com/enrolled/courses/intro-to-data-visualization-with-python) a beginner friendly course for free.
  - [Data Visualization with Python: Seaborn](https://www.codecademy.com/enrolled/courses/data-visualization-with-python-seaborn) a beginner friendly course for free.
  - See more [Python related](https://www.codecademy.com/search?query=Python) materials (you can select "Free" and/or "Beginner" filter on the left side of the page).

## LeetCode

LeetCode is a platform for practicing coding problems and preparing for technical interviews. It has a large collection of coding problems, ranging from easy to hard, and covers various topics such as algorithms, data structures, and system design.

- [LeetCode](https://leetcode.com/) - The main website for LeetCode. You can create an account and start solving problems.
  - [A few patterns](https://blog.algomaster.io/p/15-leetcode-patterns) appearing in LeetCode problems. (see the related [YouTube video](https://www.youtube.com/watch?v=DjYZk8nrXVY)

## [Time Complexity](https://github.com/Konczer/ComputationalThinkingWithPython/blob/main/02_ToolsResourcesComplexity/TimeComplexity.ipynb) 

## Wolfram blogs, Computational essays

- [Writing a Computational Essay](https://www.wolframcloud.com/obj/Expositions/Published/ComputationalEssayGuidelines)
- [Computational Essays examples](https://notebookarchive.org/collection-pod?collection=computational-essays)
- Enhanced and upgraded previous student projects:
    - [Using basic attributes to predict stellar spectral classes](https://community.wolfram.com/groups/-/m/t/2988252)
    - [Predicting whether a mushroom is poisonous or edible using five variables](https://community.wolfram.com/groups/-/m/t/2952324)
    - [Constructing universities dataset and showing some queries examples](https://community.wolfram.com/groups/-/m/t/2988279)
- [What is a Computational Essay?](https://writings.stephenwolfram.com/2017/11/what-is-a-computational-essay/) - A lengthy blog post explaining what a computational essay is and how to write one.