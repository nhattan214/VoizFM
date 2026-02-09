# ⚡ VoizFM Data Analysis Project

## 1. Project Overview
The audiobook company [VoizFM](https://voiz.vn/) currently lacks a personalization scheme for customers. They
have tracked and collected data from users’ answer to survey and their listening time. The data
used in this project is extracted based on users who have answered the app’s survey
only, and the app’s user acquisition target is set according to the demography của
paid user.

The main tasks of this project are:
* Analyse the user demography
* Analyse the users’ interests based on their answers to the survey
* Analyse the listening behavior of users
* Derive insights from the analysis using modern statistical method so that a personalization plan can be developed in the future.



---

## 2. Dataset
* **Source:** [VoizFM](https://voiz.vn/), provided by the company's technical team.
* **Description:** Reports of users' basic information (gender, date of birth), their scores to each categories of books, listening time in seconds.
* **Records:** 1162 VIP users and 1222 Free users. There are 25 categories available in the given data.

---

## 3. Tools and Libraries
* **Python 3:** `Pandas`, `NumPy`, `Seaborn`, `Matplotlib`


---

## 4. Methodology
* User demography analysis: Analysing age distribution, gender distribution, their preferences of reading voice. Analysing the similarity between "Free user" demography and "Vip user" demography by Bhattacharyya distance [1]
* Analysing the user's rating for categories and their corresponding listening time to those categories by merging/joining dataframes, to find the correlation between their ratings and actual listening behavior. Positive correlation will indicate the reliability of the current tracking method used in the app.


[1] Bhattacharyya, A. . “On a measure of divergence between two statistical populations defined
by their probability distributions”. Bulletin of the Calcutta Mathematical Society. 35: 99–109, Mar
1943.

---

## 5. Results & Key Findings
* The two user distributions are very similar in terms of distribution shape. Indeed, most users fall in the range of 23-34.
There are more VIP users than Free users from the age of 30 onwards, as they have stable income
and more willing to pay for VIP services. The opposite trend can be seen for the age group from
29 backward, as they are mostly students with less or no stable income. The user demographic of
both free plan and VIP plan are very similar in terms of age and gender types. There are mostly ‘younger’ users (<35 in terms of age).
* For most user groups, several categories show a strong positive Pearson correlation. This
indicates that users who liked these categories also tend to spend more time listening to
content within those categories. This is a good sign that user preferences, as indicated by the
survey, align well with their actual listening behavior for many content types.
* The core content pillars (“Truyện ngắn - Tản văn”, “Kinh điển”, “Tâm linh”, “Đầu
tư làm giàu”) are popular across the user base. The user survey is generally consistent with
the corresponding listening time, which shows that users honestly participated in the survey.
* Targeting the 23-39 age range is crucial for overall engagement.
* Older demographics (40+) are a valuable segment for VIP users, suggesting potential for
tailored strategies.
* Female users are the primary drivers of listening time.

**Review and endorsement** from the company's CEO for this project can be found in the recommendation section at [my LinkedIn](https://www.linkedin.com/in/pntan/)

## 6. How to run
* Installed required libraries, and Jupyter notebook (This notebook can also be run on GoogleColab)
* Clone/Download this whole project
  
