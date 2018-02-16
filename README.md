# Rmarkdown homework assignment for BIOL319
## Due as a pull request on Monday, February 19, 2017 before 11:59 pm

The **goal of this assignment** is to help you continue to learn to use R and RStudio to analyze and visualize ecological data, doing so in the context of a version-controlled workflow, and submitting your work as a Pull Request on GitHub. This time we are focusing on doing cross-site comparisons of the mass of litter of a particular functional group across all sites, and using a statistical test to determine if the differences we visualize are significant.

**General overview:** You will edit the exiting 'Analysis.Rmd' script for this assignment. It should read in the `ltr_massdata.csv` file that is in the `data` directory, use the `subset()` function to subset one functional group from that data, and then plot those data as a boxplot, with site on the x axis and dry mass on the y axis (more details below). Then you will use an appropriate statistical test to see if the differences you see (or don't see) in your plot are significant. Finally, you will need to write several paragraphs interpreting those results in the context of background you read about each of the NEON regions and sites, which is [available here](http://www.neonscience.org/field-sites/field-sites-map/list). For example, [here's a description](http://www.neonscience.org/field-sites/field-sites-map/BART) of the Bartlett Experimental Forest (short ID: BART).

Please follow the instructions carefully and read them all before getting started.

This third assignment will be worth 10 points. The grading breakdown will be as follows:

* 5 points - Completes all required steps (as outlined below)
* 2.5 points - R markdown script is appropriately commented and well organized
* 2.5 points - Appropriate use of git to version control the steps, including adding and committing the appropriate files at the specific steps below, and writing informative and appropriately formatted commit messages

You must submit your work as a Pull Request to the class organization ('2018-usfca-biol-319-spring') on GitHub by 11:59 pm on Monday, February 19 for full credit. Late assignments will not be accepted, since we will be peer reviewing each other's code after it is submitted.

Steps:

1. Fork this repository to your own GitHub account.
2. On your laptop, in RStudio, select File > New Project...
3. Choose 'Version Control', then 'git', then paste the URL from your fork and hit tab
4. This will autofill the project name, you can choose where this repository folder will be on your laptop
5. Select 'Open in New Session', then 'Create Project'
6. This should download the repository from GitHub and set up a new project for you in RStudio
7. Now, in contrast to last week, we'll be working in the `Analysis.Rmd` file instead of an R script. So, just open the existing file (look for it in the file browser tab in the lower right-hand corner of RStudio). In this script, in addition to filling in a paragraph or two in each of the sections (Introduction, Methods, Results, Discussion), you will need to create an appropriately labeled boxplot comparing mass of one functional group of litter across all sites in the dataset. To do this, you will need to create and write the appropriate R code to:
  * Read in the `ltr_massdata.csv` dataset from the `data` directory
  * Use the `subset()` function to select all measurements from only one litter type from the following: "Flowers", "Leaves", "Mixed", "Needles", "Other", "Seeds", "Twigs/branches", "Woody material".
  * Create a properly titled and labelled boxplot with the variable `siteID` on the x axis and `dryMass` on the y axis. 
8. Add and commit your R markdown script as you work on it.
9. After you have created the plot, you should add an R code chunk in your R markdown document to apply an appropriate statistical test to determine if there are significant differences in mass of your chosen litter type across NEON sites. You should report the type of test you used, the p-value it returned, and interpretation of what this p-value means about the data you plotted.
10. In the discussion section, explain what you think could be the ecological reason for the differences or lack of differences that you observed, based on your reading of the overview information about each of the sites on the NEON website. You don't have to have the right answer (if there even is one), but the goal is for you to apply ecological thinking to infer why you observe different patterns in the data. Think about type of vegetation that grows at each site, its climate, etc.
11. Add and commit your Rmd file when you are done.
12. Knit your Rmd file to a docx and commit this docx as well.
13. Push your commits back to your repository on GitHub.
14. Open a pull request back to the class repository to submit your assignment.
15. Be sure to write [meaningful commit messages](https://chris.beams.io/posts/git-commit/) and a descriptive Pull Request title and description.

Don't hesistate to ask questions on Piazza as you work!
