Project 1: Exploring climate data of Singapore

Project title: Imapact of Climate Change on Energy Cost for Households in Smaller Dwelling Units

### Contact
Github: https://github.com/MrKiasu/

### Problem Statement
Climate change is affecting Singapore in the form of rising temperature and rainfall. How does this impact our electricity consumption? And if so, how much will the cost impact households with lower income? 
This project aims to make recommendations to policymakers in the Singapore Public Service in order to help support households with lower income.

### Datasets
|Filname|Description|Source|
|---|---|---|
rainfall-monthly-total.csv | Monthly total rainfall in Singapore | NEA, https://beta.data.gov.sg/datasets/1399/view
rainfall-monthly-number-of-rain-days.csv | Monthly number of rain days in Singapore | NEA, https://beta.data.gov.sg/datasets/1398/view
relative-humidity-monthly-mean.csv | Average monthly relative humidity in Singapore | NEA, https://beta.data.gov.sg/datasets/1404/view
surface-air-temperature-monthly-mean.csv | Average monthly surface air temperature in Singapore | NEA, https://beta.data.gov.sg/datasets/1419/view
wet-bulb-temperature-hourly.csv | Average hourly wet bulb temperature in Singapore | NEA, https://beta.data.gov.sg/datasets/1423/view
T3.5 - Average Monthly Household Electricity Consumption by Planning Area & Dwelling Type.csv | Average Monthly Household Electricity Consumption by Planning Area & Dwelling Type in Singapore | EMA, https://www.ema.gov.sg/resources/singapore-energy-statistics
T5.1 - Electricity Tariffs.csv | Average monthly electricity tariffs in Singapore | EMA, https://www.ema.gov.sg/resources/singapore-energy-statistics
average-houshold-size-and-income.csv | Average household size and income in Singapore |DOS, https://www.singstat.gov.sg/publications/reference/cop2020/cop2020-sr2/census20_stat_release2


### Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|**year**|*integer*|rainfall-monthly-total|Year| 
|**month**|*integer*|rainfall-monthly-total|Month|
|**total rainfall**|*float*|rainfall-monthly-total|The monthly total rainfall recorded at the Changi Climate Station in mm(millimeters)|
|**rainy_days**|*float*|rainfall-monthly-total|The number of rain days (day with rainfall amount of 0.2mm or more) in a month recorded at the Changi Climate Station.|
|**wet bulb temperature**|*float*|wet-bulb-temperature-hourly|Average of the hourly wet bulb temperature recorded at the Changi Climate Station in degree Celsius|
|**kwh_per_acc**|*float*|T3.5 - Average Monthly Household Electricity Consumption by Planning Area & Dwelling Type|Average Annual Household Electricity Consumption in kilowatt hours|
|**dwelling_type**|*string*|T3.5 - Average Monthly Household Electricity Consumption by Planning Area & Dwelling Type|Type of dwelling units (e.g. 3-room flat)|
|**elect_tariffs**|*float*|T5.1 - Electricity Tariffs|Annual electricity tariffs (weighted average) in cents/kWh|
|**household_income**|*float*|average-houshold-size-and-income|Average household income|
|**household_size**|*float*|average-houshold-size-and-income|Average household size|


### Conclusion
Climate change causes rising temperatures (surface air) and rainfall, leading to higher wet bulb temperature.
With increasing wet bulb temperature, household electricity consumption is expected to increase with the increased use of air conditioning and fans.
It is also found that electricity cost is a higher proportion of income for those staying in smaller dwelling units despite using less electricity.

Therefore, we expect climate change to disproportionally impact those staying in smaller dwelling in terms of electricity cost.


### Recommendation
A three-pronged approach is recommended:
1. To mitgate climate change, long term policies are recommended (e.g. to reduce waste).
2. Electricity tariffs can be scaled such that those who consume more electricity should be charged a higher tariffs.
3. Provide subsidies directly to those staying in smaller dwelling units (1-3 room flats) 




---



#### Provided Data

There are 2 datasets included in the [`data`](./data/) folder for this project. These correponds to rainfall information. 

* [`rainfall-monthly-number-of-rain-days.csv`](./data/rainfall-monthly-number-of-rain-days.csv): Monthly number of rain days from 1982 to 2022. A day is considered to have “rained” if the total rainfall for that day is 0.2mm or more.
* [`rainfall-monthly-total.csv`](./data/rainfall-monthly-total.csv): Monthly total rain recorded in mm(millimeters) from 1982 to 2022

Other relevant weather datasets from [data.gov.sg](data.gov.sg) that you can download and use are as follows:

* [Relative Humidity](https://data.gov.sg/dataset/relative-humidity-monthly-mean)
* [Monthly Maximum Daily Rainfall](https://data.gov.sg/dataset/rainfall-monthly-maximum-daily-total)
* [Hourly wet bulb temperature](https://data.gov.sg/dataset/wet-bulb-temperature-hourly)
* [Monthly mean sunshine hours](https://data.gov.sg/dataset/sunshine-duration-monthly-mean-daily-duration)
* [Surface Air Temperature](https://data.gov.sg/dataset/surface-air-temperature-mean-daily-minimum)

**Make sure you cross-reference your data with your data sources to eliminate any data collection or data entry issues.**

#### Additional Data
You can also use other datasets for your analysis, make sure to cite the source when you are using them.

---

### Deliverables

All of your projects will comprise of a written technical report and a presentation. As we continue in the course, your technical report will grow in complexity, but for this initial project it will comprise:
- A Jupyter notebook that describes your data with visualizations & statistical analysis.
- A README markdown file the provides an introduction to and overview of your project.
- Your presentation slideshow rendered as a .pdf file.
**NOTE**: Your entire Github repository will be evaluated as your technical report. Make sure that your files and directories are named appropriately, that all necessary files are included, and that no unnecessary or incomplete files are included.

For your first presentation, you'll be presenting to a **non-technical** audience. You should prepare a slideshow with appropriately scaled visuals to complement a compelling narrative. **Presentation duration will be 6 minutes.**

---

### Technical Report Starter Code

Future projects will require you to decide on the entire structure of your technical report. Here, we provide you with [starter code](./code/starter-code.ipynb) in a Jupyter notebook that will help to guide your data exploration and analysis. **If you choose to edit the core structure of this notebook, make sure you don't exclude any of the requested operations**.

---

### Suggested Resources

Here's a link on [how to give a good lightning talk](https://www.semrush.com/blog/16-ways-to-prepare-for-a-lightning-talk/), which provides some good recommendations for short presentations.

[Here's a great summary](https://towardsdatascience.com/storytelling-with-data-a-data-visualization-guide-for-business-professionals-97d50512b407) of the main points of the book _Storytelling with Data_, which I can't recommend enough. [Here's a blog post](http://www.storytellingwithdata.com/blog/2017/8/9/my-guiding-principles) by the author about his guiding principles for visualizations.

---

### Submission

**Materials must be submitted through your GitHub account repo shared with the Teaching Team by scheduled due date.**

Your technical report will be hosted on github.com Make sure it includes:

- A README.md (that isn't this file)
- Jupyter notebook(s) with your analysis (renamed to describe your project)
- Data files
- Presentation slides
- Any other necessary files (images, etc.)

---

### Presentation Structure

- **Presentation Time: 6 minutes**
- Use Google Slides or some other visual aid (Keynote, Powerpoint, etc).
- Consider the audience. Assume you are presenting to a non-technical audience (executives with the College Board, school administrators, admissions counselors, State officials, etc.).
- Start with the **data science problem**.
- Use visuals that are appropriately scaled and interpretable.
- Talk about your procedure/methodology (high level, **CODE IS ALWAYS INAPPROPRIATE FOR A NON-TECHNICAL AUDIENCE**).
- Talk about your primary findings.
- Make sure you provide **clear recommendations** that follow logically from your analyses and narrative and answer your data science problem.

Be sure to rehearse and time your presentation before class.

---

### Rubric
Teaching team will evaluate your project using the following criteria.  You should make sure that you consider and/or follow most if not all of the considerations/recommendations outlined below **while** working through your project.

**Note:** Presentation and codes will be prepared and submitted by each student individually.

**Scores will be out of 21 points based on the 7 items in the rubric.** <br>
*3 points per section*<br>

| Score | Interpretation |
| --- | --- |
| **0** | *Project fails to meet the minimum requirements for this item.* |
| **1** | *Project meets the minimum requirements for this item, but falls significantly short of portfolio-ready expectations.* |
| **2** | *Project exceeds the minimum requirements for this item, but falls short of portfolio-ready expectations.* |
| **3** | *Project meets or exceeds portfolio-ready expectations; demonstrates a thorough understanding of every outlined consideration.* |

**Project Organization**
- Are modules imported correctly (using appropriate aliases)?
- Are data imported/saved using relative paths?
- Does the README provide a good executive summary of the project?
- Is markdown formatting used appropriately to structure notebooks?
- Are there an appropriate amount of comments to support the code?
- Are files & directories organized correctly?
- Are there unnecessary files included?
- Do files and directories have well-structured, appropriate, consistent names?

**Clarity of Message**
- Is the problem statement clearly presented?
- Does a strong narrative run through the project?
- Does the student provide appropriate context to connect individual steps back to the overall project?
- Is it clear how the final recommendations were reached?
- Are the conclusions/recommendations clearly stated?

**Python Syntax and Control Flow**
- Is care taken to write human readable code?
- Is the code syntactically correct (no runtime errors)?
- Does the code generate desired results (logically correct)?
- Does the code follows general best practices and style guidelines?
- Are Pandas functions used appropriately?
- Does the student demonstrate mastery masking in Pandas?
- Does the student demonstrate mastery sorting in Pandas?

**Data Cleaning and EDA**
- Does the student fix data entry issues?
- Are data appropriately labeled?
- Are data appropriately typed?
- Are datasets combined correctly?
- Are appropriate summary statistics provided?
- Are steps taken during data cleaning and EDA framed appropriately?

**Visualizations**
- Are the requested visualizations provided?
- Do plots accurately demonstrate valid relationships?
- Are plots labeled properly?
- Plots interpreted appropriately?
- Are plots formatted and scaled appropriately for inclusion in a notebook-based technical report?

**Research and Conceptual Understanding**
- Were useful insights gathered from outside sources?
- Are sources clearly identified?
- Does the student provide appropriate interpretation with regards to descriptive and inferential statistics?

**Presentation**
- Is the problem statement clearly presented?
- Does a strong narrative run through the presentation building toward a final conclusion?
- Are the conclusions/recommendations clearly stated?
- Is the level of technicality appropriate for the intended audience?
- Is the student substantially over or under time?
- Does the student appropriately pace their presentation?
- Does the student deliver their message with clarity and volume?
- Are appropriate visualizations generated for the intended audience?
- Are visualizations necessary and useful for supporting conclusions/explaining findings?

In order to pass the project, students must earn a minimum score of 1 for each category.
- Earning below a 1 in one or more of the above categories would result in a failing project.
- While a minimum of 1 in each category is the required threshold for graduation, students should aim to earn at least an average of 1.5 across each category. An average score below 1.5, while it may be passing, means students may want to solicit specific feedback in order to significantly improve the project before showcasing it as part of a portfolio or the job search.

### REMEMBER:

This is a learning environment and you are encouraged to try new things, even if they don't work out as well as you planned! While this rubric outlines what we look for in a _good_ project, it is up to you to go above and beyond to create a _great_ project. **Learn from your failures and you'll be prepared to succeed in the workforce**.
