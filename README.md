# Real / Fake Job postings
This project includes visualizing the data and building a model to predict if any job posting is real or fake given the details about the posting. I ended up using this dataset because nowadays many fraudulent companies post fake jobs to collect candidates’ personal data and try to misuse it. It would be a helpful tool if the candidate can make sure if any given posting is genuine or not.
The steps in this project involved normalising the raw dataset given by the university of the Aegean | Laboratory of Information & Communication Systems Security. I studied the data, cleaned the data, performed exploratory data analysis and created a predictive logistic regression model that uses data columns as parameters to predict which jobs are fraudulent and which are real.

## Data Description:
The dataset consists of 17,880 observations and 18 features. The data is a combination of integer, binary and textual datatypes. A brief definition of the main attributes is given below:
- Title – Description of the job position. 
- Location - Geographical location of the job
- Department – Information about the department of the offered job 
- Company profile - A brief description of the company.
- Requirements - Pre-requisites to qualify for the job
- Telecommuting - work from home or remote work allowed or not in the job. 
- Benefits – Enlisted benefits provided by the job
- Required experience – It can be Executive, Entry level, Intern, etc. 
- Has company logo - Does the job posting have a company logo
- Required education – It can be Doctorate, Master’s Degree, Bachelor, etc.
- Industry - The industry the job posting is relevant to (Automotive, IT, Health care etc.)
- Function – Information about the Job’s functionality (Consulting, Engineering, Research, Sales etc.) 
- Employment Type - Full-type, Part-time, Contract, etc.


## Analysis Methods:
Data was ingested into SQLite and then pulled from it into the python notebook for further analysis. Python libraries, matplotlib and seaborn were used for the exploratory data analysis. Random Forest model was built to predict the output in binary form – the job is fake or real.