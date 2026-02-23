# Spring 2026 Data Challenge Instructions

## Foreword

The Data Challenge is a biannual event in which teams of participants are given a dataset to analyze and make predictions about, along with a series of guiding questions to orient the analysis. This event provides an opportunity for students to gain practice in working with real data, conducting a meaningful and rigorous analysis, and communicating the results clearly and concisely.

Each project is judged by the presentation, methodology, and written report. Teams may earn substantial additional points for completing the optional prediction component through the development and evaluation of a predictive model. The emphasis of this Data Challenge is on clear explanations of the conclusions and the underlying methodology. Your presentation may also include any exploratory analysis of the dataset, potential weaknesses of your model or methodology, and/or future improvements you would make to your work.

## Introduction to the Data Challenge

This semester’s Data Challenge is centered around statistical consulting. Statisticians are often asked to work in consulting roles on academic and business problems (for example, UW–Madison’s [Statistical Consulting group](https://stat.wisc.edu/statistical-consulting/)), and in this challenge, you will step into that role.

You will act as a data consultant for a business owner preparing to open a new business. Using a comprehensive business and customer review dataset comprising 5 files containing close to 7 million reviews and 150 thousand businesses across multiple metropolitan areas, your task is to help the owner make informed, evidence-based decisions before and after their grand opening.

Rather than focusing on a single question, this challenge is designed to reflect the kind of decisions consultants actually face: identifying which business attributes are most likely to matter, making predictions about post-opening performance, and communicating recommendations clearly to a non-technical client. In the final stage, you will translate your analysis into a concise dashboard, choosing the plots and metrics that best capture what a business owner should pay attention to.

This challenge emphasizes not only statistical analysis, but also prioritization, interpretation, and communication — all core parts of doing statistics in practice.

### Part 1: The Client Presentation & Dashboard (Presentation)

Your statistical analysis is only as good as your ability to communicate it. Your primary deliverable is a presentation centered around a concise informative "dashboard" designed specifically for your non-technical client. 

Your dashboard is strictly constrained to:

- A maximum of 5 plots/visualizations

- A maximum of 5 key metrics that you believe are most helpful to business owners

What to analyze for your presentation: What attributes do successful businesses share? You must decide exactly what information is most critical for a business owner to monitor to be successful. Teams must define and justify what constitutes “success.” We recommend comparing businesses of similar types and with similar characteristics to isolate the specific attributes that correlate with higher survival rates and better reviews.

Alongside the dashboard, your presentation must provide a clear statistical justification explaining why you chose to keep those specific plots and numbers over all other possibilities. 

### Part 2: The Predictive Component
To support your consulting recommendations with statistical evidence, you will develop a predictive model for business survival.

You will receive a subset of the business dataset in which the closure status (open vs. permanently closed) has been removed. Using the remaining information, your task is to predict whether each business in this subset is still operating.

Your model should be built using features derived from the full dataset (e.g., star ratings, number of reviews, “useful,” “funny,” and “cool” votes, check-ins, tips, user activity, or other engineered variables). A central goal of this component is to determine which signals are most informative for predicting business closure and to evaluate their relative importance.

You will train your model on 80% of the available labeled data and evaluate its performance on the remaining 20% test set. You should be able to clearly explain your modeling choices and performance metric(s).

### Evaluation & Final Grading
Your final submission will be evaluated holistically on both components. **Statistical reasoning and justification would be the focal points of your analysis and presentation. You will primarily be judged on how well you are able to provide statistical evidence and use statistical reasoning.** You will also be graded on the clarity, prioritization, and business-value of your presentation part as well as the accuracy of your predictive component.


## The Data

You can find the data [here](https://drive.google.com/drive/folders/1gEC4bbn9RDwlY8ewzPHMXn0LphJeDHi3?usp=sharing). The datasets are stored using `.parquet` file types, which are very efficient for large datasets such as ours. They can be easily read just like `.csv` into Python and R environments. 

The files are named as follows:
- business_y_removed.parquet
- review.parquet
- user.parquet
- checkin.parquet
- tip.parquet

Please refer to the documentation for more information.

## Important Dates

**February 23, 2026** Data Challenge Begins

**March 2, 2026** In-person Help Session

**March 6, 2026** Mid-point checkpoint

**March 13, 2026** Report, and Code are due by 11:59pm (Presentation slides not required at this point)

**March 16, 2026** Final Presentations


---
GROUPS MAY HAVE UP TO 4 MEMBERS . . .  NO MORE
---


## Awards:
Certificates will be given for the following categories:
- Best Oral Presentation
- Best Written Report
- Most Accurate Model
- Best Visualizations
- Best Overall Project

Teams will be judged by department faculty and graduate students. You will receive official certificates for the awards, and your team photos will be shared on our club’s social media pages. The team that wins **Best Overall Project** will earn spots on the UW–Madison team for MUDAC, a regional statistical analysis competition, with full travel funding provided.


## Presentations:
Your group will prepare a roughly ten-minute (subject to change) presentation of your data analysis, followed by questions from the judges and audience. The goal of the presentation is to practice presenting statistical findings in a concise and clear manner. The presentation should include key evidence (e.g. plots, tables, inferential methods, etc.) that support your findings. Your presentation must be clear and precise enough that the audience will be able to understand which statistical analyses you used and how you have reached your conclusions.

The requirements for the presentation are as follows:
-  Due to time constraints, the ten-minute time limit will be strictly enforced.  While we will provide time cards and warnings for you during the presentation, it is ultimately your responsibility to rehearse your presentation so that it stays under ten minutes. 
-  Each member of your group must speak for at least 1 minute during the ten-minute presentation. 
- All members of the group must work on the presentation and be prepared to answer 1-3 short questions about the presentation from the audience (including the judges and other participants).

The exact time of your group’s presentation will be determined randomly on the day of the presentation.


## Written Report:

Your group must submit a one to two-page report of the data analysis. In particular, the report should include (1) your **overall findings**, (2) relevant and important **evidence** for your findings (e.g. plots, tables), and (3) important **details of your statistical analysis** (e.g. type of model used, inferential quantities, outliers, leverage points, modeling assumptions, etc.). Your report should be detailed enough that any data scientist can read it and replicate your analysis.

The requirements for the executive report are as follows: 

- Typed in 12-inch Times New Roman or Arial, single-spaced, 1-inch margins 
- Include all relevant figures/tables, equations, and references 
- Must be legible 
- Must not exceed two pages 
- You may follow any reasonable guidelines for formatting the references (Ex. MLA, APA, Chicago Manual of Style, etc.)


  ## Submission

  All submissions (including midpoint checkppoint, final, and presentation slides) must be made through the dedicated submission form here: https://docs.google.com/forms/d/e/1FAIpQLSc5cdUjYcT3i0Lcs2IuTwAH1-vzN9X7fhUYX2E4Z7c4-dy0Xw/viewform?usp=publish-editor

  Submissions must be recieved by 11:59pm on the date they are due (or 6pm on 16th March in case of presentation slides). Late submissions will not be accepted out of fairness to all teams. Submit well ahead of time to avoid last minute technical issues.


  ### Checkpoint submission

  Submit ONE zipped folder with your team name in the file name containing the following:

  - Exploratory Code Analysis
  - A document explaining your code and findings so far. This does not have to be as polished as the final executive report
 
  ### Final Submission

  Submit ONE zipped folder with your team name in the file name containing the following:

  - All of your code files
  - Executive Report (PDF)
  - requirements.txt (this text file should include all the external libraries/frameworks that your code uses)
  - AI Tool Usage (PDF)

  

  


  # Data Challenge Rubric (Spring 2026)

| Category | Criteria | Description | Points |
|----------|---------|------------|-------|
| **Presentation** (30 pts) | P1 | Communicates key messages and conclusions clearly, leaving the audience with a strong understanding of the findings. | 6 |
|  | P2 | Uses visuals (plots, charts, tables) that are clear, relevant, and easy to follow. Explanations are concise and accessible. | 6 |
|  | P3 | Demonstrates that methods are statistically sound; addresses strengths and weaknesses. Interprets results correctly and highlights insights. | 6 |
|  | P4 | Provides strong evidence and logical reasoning to support conclusions. Connects analysis to findings effectively. | 6 |
|  | P5 | Delivers the presentation clearly and engagingly. Maintains audience understanding throughout. | 6 |
| **Methodology** (40 pts) | M1 | Introduces the dataset, context, and purpose of the analysis. Includes a well-defined thesis or research question. | 8 |
|  | M2 | Justifies the choice of data analysis methods or predictive techniques, explaining why they fit the problem or dataset. | 8 |
|  | M3 | Explains key findings clearly and concisely, including parameter estimates (if applicable) and their significance. Avoids unnecessary output. Interprets results in accessible terms. | 8 |
|  | M4 | Assesses strengths and weaknesses of chosen methods, checking assumptions and diagnostics (e.g., overfitting, bias-variance, validation performance). | 8 |
|  | M5 | Evaluates predictive or explanatory accuracy using appropriate metrics and validation. | 8 |
| **Write-up** (10 pts) | W1 | Presents a concise, well-structured one–two page executive report that summarizes methods, key findings, and evidence in an accessible way. | 5 |
|  | W2 | Provides figures, tables, and references as needed for replication and clarity. | 5 |
| **Prediction Accuracy** (20 pts) | A1 | For teams that include forecasting or prediction: evaluates the out-of-sample accuracy of the model using appropriate metrics (e.g., RMSE, MAE, MAPE). | 10 |
|  | A2 | Demonstrates robustness of the predictive model (e.g., cross-validation, sensitivity checks) and interprets the results effectively. | 10 |

**Total: 100 points**


## Rules and Academic Integrity

Each student assumes the responsibilities of an active participant in UW–Madison’s community of scholars. All academic work and behavior are held to the highest standards of integrity. Academic misconduct compromises the integrity of the university. Examples of misconduct include cheating, fabrication, plagiarism, sabotaging other groups’ work, unauthorized collaboration, and helping others commit these acts.

---

### Specific Guidelines

- **No copying, plagiarizing, or stealing** deliverables from other groups, students outside of the club, or the Internet.  
- You may ask other groups about general ideas or questions. However, **you cannot** ask them for help cleaning, analyzing, or interpreting the dataset.  
- **Directly copying, paraphrasing, or using existing analyses** of the competition dataset is prohibited. Examples include:  
  - Online course materials  
  - Blog posts or published notebooks  
- You are **encouraged** to browse for background information. Using external resources to provide context is acceptable as long as you give proper attribution and ensure the analysis itself is your own work.  
- Your team’s analysis must be **original** and reflect your own effort. In industry terms: *do not steal others’ intellectual property*.  
- You may not ask anyone outside your group to perform any part of the analysis on your behalf.  

---

### Use of AI Tools

AI tools (e.g., ChatGPT, Copilot) are permitted under **standard academic integrity policies**. We want participants to gain *real-world experience*, where the use of AI is increasingly common.  

However:  
- If AI is used, your team must still be able to **explain, justify, and defend** all decisions made in your analysis.  
- Failure to demonstrate understanding of your own work because of overreliance on AI will be considered a **serious penalty**. It will heavily impact the quality assessment of your project.
- You must disclose any AI tools used, how you used it, and the prompts you entered, in a standalone document titled "AI Tool Usage".

--- 
### Use of API Tools

Participants are permitted to use external APIs (e.g., Hugging Face or similar platforms) to access machine learning models, provided that these models are general-purpose and not already specifically trained or fine-tuned on the challenge dataset. This policy aligns with standard research and industry practices, ensuring participants can leverage established tools without “reinventing the wheel,” while maintaining fairness and originality in the development of solutions.
