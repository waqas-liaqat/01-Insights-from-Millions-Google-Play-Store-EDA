# **Exploratory Data Analysis (EDA) Project**

## **Insights from Millions: Google Play Store EDA**

---

To see [Live at Kaggle](https://www.kaggle.com/code/muhammadwaqas630/insights-from-millions-google-play-store-eda/notebook)

---

## **Table of Contents**
1. [Project Overview](#project-overview)
2. [Dataset Information](#dataset-information)
3. [Data Cleaning](#data-cleaning)
4. [Exploratory Data Analysis](#exploratory-data-analysis)
5. [Deeper Observations](#Deeper-Observations)
6. [Questions & Answers](#Questions-&-Answers)
7. [Technologies Used](#technologies-used)
8. [Acknowledgments](#Acknowledgments)
9. [Connect with Me](#Connect-with-Me)

---

## **Project Overview**

This project dives deep into the world of Google Play Store apps through an extensive Exploratory Data Analysis (EDA). By examining various features such as app categories, user ratings, review counts, installs, and more, this analysis uncovers valuable trends and insights into the Play Store ecosystem.

### **Objective:**
The primary objective of this project is to derive significant insights from the dataset, helping app developers and other stakeholders understand customer behavior and app dynamics. This can serve as a guide to inform the development of future applications and business strategies.

---

## **Dataset Information**

- **Dataset:** Google Play Store Apps
- **Time Period:** Data collected in June 2021
- **Source:** [Google Playstore Dataset](https://www.kaggle.com/datasets/gauthamp10/google-playstore-apps)
  
### **Dataset Columns Overview**

| **Column Name** | **Description** |
|:---:|:---:|
| App Name | Name of the app |
| App Id | Package name |
| Category | App category |
| Rating | Average user rating |
| Rating Count | Total number of ratings |
| Installs | Approximate install count |
| Minimum Installs | Minimum number of installs |
| Maximum Installs | Maximum number of installs |
| Free | App pricing (Free or Paid) |
| Price | Price of the app (if paid) |
| Currency | Currency used for pricing |
| Size | App size |
| Minimum Android | Minimum Android version supported |
| Developer Id | Developer's ID in Play Store |
| Developer Website | Developer's website |
| Developer Email | Developer's email |
| Released | App release date |
| Last Updated | Last app update date |
| Content Rating | Target audience of the app |
| Privacy Policy | App privacy policy |
| Ad Supported | Whether the app supports ads |
| In-App Purchases | Whether the app has in-app purchases |
| Editors Choice | Whether the app is an Editors' Choice app |
| Scraped Time | Timestamp of data collection |

---

## **Data Cleaning**

The following steps were taken to clean and preprocess the dataset:

- **Handling Missing Values:**
  - Missing app names and minimum Android versions were removed due to their low impact.
  - Null values in the **Size** column were filled with "Varies with device" since this was consistent with the **Minimum Android** version.
  - Missing **Currency** values were replaced with "XXX" as they corresponded with free apps (Price = 0).
  - Other missing values in columns like **Installs**, **Rating**, and **Released** were minimal, so these rows were dropped to preserve dataset integrity.

- **Duplicate Removal:**
  - No duplicates were found.

- **Anomalies:**
  - Instances where the **Last Updated** date was earlier than the **Released** date were corrected or removed.

- **Feature Engineering:**
  - Converted the **Size** column to a numeric format.
  - Transformed **Released** and **Last Updated** into datetime objects.
  - Dropped irrelevant columns like **Scraped Time** as they added no analytical value.

---

## **Exploratory Data Analysis**

### **Key Insights:**

- **App Size:**
  - Minimum app size: 3KB, Maximum size: 1536MB, Average size: 10MB.
  
- **App Pricing:**
  - More than 75% of apps are free.

- **Release Timeline:**
  - The first app was released on **2010-01-28**, and the most recent app (as of the dataset) was released on **2021-06-16**.

- **Update Anomalies:**
  - Anomalous data found where apps were updated before being released, e.g., the oldest update was recorded on **2009-02-09**.

---

### **Deeper Observations:**

- **App Categories:**
  - There are 48 distinct categories, with **Education** having the most apps.

- **Download Trends:**
  - Most apps have download counts in the hundreds.
  - **Tools, Communication, Productivity, Photography**, and **Video Players & Editors** are the top categories in terms of downloads.

- **Content Rating:**
  - Apps with a content rating of **"Everyone"** have the highest install base, followed by **Teen**-rated apps.

---

## **Questions & Answers**

During the analysis, several key questions were posed to uncover trends:

1. **Is there a correlation between ratings and downloads?**
   - **Answer:** While apps with fewer downloads showed no clear relationship, highly downloaded apps tended to have better ratings.

2. **Are free apps more popular than paid ones?**
   - **Answer:** Free apps generally receive more downloads than paid ones.

3. **Which categories have the most apps and downloads?**
   - **Most Apps:** Education, Music & Audio, Tools, Business, and Entertainment.
   - **Most Downloads:** Tools, Communication, Productivity, Photography, and Video Players & Editors.

4. **Does the price of an app affect its rating?**
   - **Answer:** There is no direct relationship between app price (free vs. paid) and ratings.

5. **How does app size relate to installs?**
   - **Answer:** Apps smaller than 200MB tend to have higher downloads.

6. **Do app release years impact downloads?**
   - **Answer:** Apps released in **2015** saw the highest download counts, and **2020** had the highest number of app releases.

---

## **Technologies Used**

The following technologies were employed in this project:

- **Python 3.12.0**
- **Pandas** for data manipulation
- **Matplotlib** & **Seaborn** for visualizations
- **Jupyter Notebook** for development

---

## **Acknowledgments**

Special thanks to **Kaggle** for providing the dataset and to **Dr. Ammar Tufail** for inspiration and guidance throughout this project.

---


## **Connect with Me**

To connect with me or explore my work, feel free to reach out through the following platforms:

[![Email](https://img.shields.io/badge/Email-waqasliaqat630%40gmail.com-red)](mailto:waqasliaqat630@gmail.com)  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Muhammad%20Waqas%20Liaqat-blue)](https://www.linkedin.com/in/muhammad-waqas-liaqat/)  
[![GitHub](https://img.shields.io/badge/GitHub-Waqas%20Liaqat-black)](https://github.com/waqas-liaqat)  
[![Kaggle](https://img.shields.io/badge/Kaggle-Muhammad%20Waqas-brightblue)](https://www.kaggle.com/muhammadwaqas630)
