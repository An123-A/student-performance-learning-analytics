# Student Performance: A Learning Analytics Project
## Project overview 
This project uses the Student Performance dataset from the UCI Machine Learning Repository to explore factors related to secondary school students' academic performance. The dataset contains information about students' demographic characteristics, family backgrounds, study habits, school experiences, social behaviors, attendance, and academic grades. For this project, I use the Mathematics course dataset ('student-mat.csv'), which contains 395 student records and 33 variables. The purpose of this project is to document the dataset clearly and systematically so that other researchers can understand, access, interpret, and potentially reuse the data for learning analytics and educational research. 
## Research Questions 
This project is guided by the following questions:
1. How are students' study habits and school attendance associated with academic performance?
2. How do family and social factors relate to students' final grades?
3. Which student characteristics may be useful for understanding differences in academic performance? 

## Dataset Overview
### Data Source
The data used in this project come from the **Student Performance** dataset available through the UCI Machine Learning Repository. The dataset was created by Paulo Cortez and contains student achievement data collected from two Portuguese secondary schools. The data were obtained from school reports and questionnaires and include demographic, social, family, school-related, and academic information.
- **Dataset:** Student Performance
- **Creator:** Paulo Cortez
- **Repository:** UCI Machine Learning Repository
- **File used in this project:** `student-mat.csv`
- **Course:** Mathematics
- **Number of observations:** 395 students
- **Number of variables:** 33
- **Missing values:** None reported in the dataset
- **DOI:** [10.24432/C5TG7T](https://doi.org/10.24432/C5TG7T)
- **License:** Creative Commons Attribution 4.0 International (CC BY 4.0)
### File Overview
| File | Format | Description |
|------|--------|-------------|
| `student-mat.csv` | CSV | Student-level data for the Mathematics course, containing 395 observations and 33 variables. |
| `README.md` | Markdown | Documentation describing the project, dataset, metadata, methodology, data dictionary, and access information. |

## Metadata Standard
This project uses the **Data Documentation Initiative (DDI)** as the primary metadata standard. DDI is an international metadata standard designed to describe data produced in the social, behavioral, economic, and health sciences.
I selected DDI because the Student Performance dataset contains student-level educational and social science data. The standard provides a structured way to document important information such as the dataset's source, variables, data collection methods, access conditions, and information needed for data interpretation and reuse.
Following DDI principles, this README documents:
- the purpose and context of the project;
- the source and structure of the dataset;
- data collection and methodological information;
- variable names, definitions, types, and coding;
- data access, licensing, and sharing conditions; and
- information needed to support interpretation and reuse of the data.

## Methodology
### Original Data Collection
The Student Performance dataset was originally collected from two Portuguese secondary schools. According to the dataset documentation, the information was obtained using **school reports and student questionnaires**. The dataset combines academic performance measures with demographic, family, social, and school-related characteristics.
The original dataset contains data for two subjects: Mathematics and Portuguese. This project focuses only on the Mathematics dataset (`student-mat.csv`).
### Data Preparation
The Mathematics dataset contains **395 observations and 33 variables**. Each row represents one student, and each column represents a student characteristic or academic measure.
Before documenting the dataset, the file was reviewed to identify:
- the number of observations and variables;
- variable names and data types;
- categorical and numerical variables;
- coded response values;
- missing values; and
- academic outcome variables.
No missing values were identified in the Mathematics dataset.
### Analytical Approach
This project approaches the dataset from a **learning analytics** perspective. The primary academic outcome is the final Mathematics grade (`G3`), while other variables describe students' demographic characteristics, family backgrounds, study behaviors, school experiences, social behaviors, attendance, and previous academic performance.
The dataset can be used to explore relationships between these factors and students' academic performance. The current README focuses primarily on documenting the dataset and its metadata rather than making causal claims about factors that determine student achievement.
## Data Dictionary
The following data dictionary describes the 33 variables included in the Mathematics dataset. Variable definitions and coding are based on the documentation provided by the UCI Machine Learning Repository.

| Variable | Type | Description | Values / Coding |
|---|---|---|---|
| `school` | Categorical | Student's school | GP = Gabriel Pereira; MS = Mousinho da Silveira |
| `sex` | Binary | Student's sex | F = female; M = male |
| `age` | Integer | Student's age | 15–22 years |
| `address` | Binary | Home address type | U = urban; R = rural |
| `famsize` | Binary | Family size | LE3 = ≤3; GT3 = >3 |
| `Pstatus` | Binary | Parents' cohabitation status | T = living together; A = apart |
| `Medu` | Ordinal | Mother's education | 0 = none; 1 = primary; 2 = 5th–9th grade; 3 = secondary; 4 = higher education |
| `Fedu` | Ordinal | Father's education | 0 = none; 1 = primary; 2 = 5th–9th grade; 3 = secondary; 4 = higher education |
| `Mjob` | Categorical | Mother's job | teacher; health; services; at_home; other |
| `Fjob` | Categorical | Father's job | teacher; health; services; at_home; other |
| `reason` | Categorical | Reason for choosing the school | home; reputation; course; other |
| `guardian` | Categorical | Student's guardian | mother; father; other |
| `traveltime` | Ordinal | Home-to-school travel time | 1 = <15 min; 2 = 15–30 min; 3 = 30–60 min; 4 = >60 min |
| `studytime` | Ordinal | Weekly study time | 1 = <2 hrs; 2 = 2–5 hrs; 3 = 5–10 hrs; 4 = >10 hrs |
| `failures` | Integer | Number of past class failures | Number of previous failures, with higher values representing more failures |
| `schoolsup` | Binary | Extra educational support | yes; no |
| `famsup` | Binary | Family educational support | yes; no |
| `paid` | Binary | Extra paid classes for Mathematics | yes; no |
| `activities` | Binary | Participation in extracurricular activities | yes; no |
| `nursery` | Binary | Attended nursery school | yes; no |
| `higher` | Binary | Wants to pursue higher education | yes; no |
| `internet` | Binary | Internet access at home | yes; no |
| `romantic` | Binary | Currently in a romantic relationship | yes; no |
| `famrel` | Ordinal | Quality of family relationships | 1 = very bad to 5 = excellent |
| `freetime` | Ordinal | Free time after school | 1 = very low to 5 = very high |
| `goout` | Ordinal | Frequency of going out with friends | 1 = very low to 5 = very high |
| `Dalc` | Ordinal | Workday alcohol consumption | 1 = very low to 5 = very high |
| `Walc` | Ordinal | Weekend alcohol consumption | 1 = very low to 5 = very high |
| `health` | Ordinal | Current health status | 1 = very bad to 5 = very good |
| `absences` | Integer | Number of school absences | 0–93 |
| `G1` | Integer | First-period Mathematics grade | 0–20 |
| `G2` | Integer | Second-period Mathematics grade | 0–20 |
| `G3` | Integer | Final Mathematics grade | 0–20; primary outcome variable |

## Data Access and Sharing
### Access
The Student Performance dataset is publicly available through the **UCI Machine Learning Repository**. Researchers, students, and other users can access the dataset from the official repository:
[UCI Machine Learning Repository – Student Performance Dataset](https://archive.ics.uci.edu/dataset/320/student+performance)
The dataset includes both Mathematics (`student-mat.csv`) and Portuguese (`student-por.csv`) course data. This project uses only the Mathematics dataset.
### License
The dataset is distributed under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license. This license allows users to share and adapt the material, provided that appropriate credit is given to the original source.
When reusing this dataset, users should cite the original dataset:
> Cortez, P. (2008). *Student Performance* [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5TG7T
### Ethical and Privacy Considerations
The publicly available dataset does not include direct personal identifiers such as student names, addresses, or identification numbers. However, it contains demographic, family, behavioral, and academic information about students. Researchers should therefore interpret the data responsibly and avoid attempting to identify individual students.
Analyses using this dataset should also avoid treating associations as evidence of causation or using student characteristics to make unsupported judgments about individual students.

## Researcher Information
**Author:** Meilin An  
**ORCID:** [0000-0003-1983-4032](https://orcid.org/0000-0003-1983-4032)
### Dataset DOI
The original Student Performance dataset is identified by the following DOI:
**DOI:** [10.24432/C5TG7T](https://doi.org/10.24432/C5TG7T)

## Project Reflection
### Which metadata standard did I choose and why?
I chose the **Data Documentation Initiative (DDI)** as the metadata standard for this project. DDI is particularly appropriate because the dataset contains educational and social science data at the student level. It provides a structured framework for documenting the dataset's context, variables, methodology, access conditions, and information needed for interpretation and reuse.
### Which template/software did I use?
I created this README using **GitHub and Markdown**. I used the general structure recommended by **Make a README** as a guide and adapted it to meet the documentation needs of this dataset and the requirements of this project. Markdown was used to organize the document with headings, lists, links, code formatting, and tables.
### What was the most challenging part?
The most challenging part of creating the README was developing a clear and detailed **data dictionary**. Many variables in the dataset use abbreviated names and numerical or categorical codes that are not immediately understandable without documentation.
I addressed this challenge by consulting the official UCI Machine Learning Repository documentation and organizing the information into a structured table that includes each variable's name, type, description, and coding. This process helped make the dataset easier for other users to understand and reuse.
