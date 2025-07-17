# 📞 911 Calls Data Analysis Using Python

In this project, **I analyzed 911 call data from Montgomery County, Pennsylvania**, to understand **patterns in emergency calls using Python, pandas, and visualization libraries**. This helped me improve my **data cleaning, feature engineering, and data visualization skills** on real-world data.

---

## 📂 Dataset Used

I used the **911 Calls dataset from Kaggle**, which contains \~99,000 emergency call records with fields such as latitude, longitude, description, zipcode, title, timestamp, township, address, and call reason.

📌 **Dataset link :** [911 Calls Dataset on Kaggle](https://www.kaggle.com/datasets/mchirico/montcoalert)

---

## 🛠️ Tools and Libraries

* **Python**: Main language for data analysis
* **pandas**: Data cleaning and manipulation
* **numpy**: Numerical operations
* **matplotlib and seaborn**: Data visualization
* **Jupyter Notebook**: Running and documenting analysis step-by-step

---

## 🚩 What I Have Done

✅ **Imported and explored the data:**

* Loaded the dataset using pandas and checked the structure using `.info()` and `.head()`.
* Identified missing values and data types.

✅ **Feature Engineering:**

* Extracted the **Reason for 911 calls (EMS, Fire, Traffic)** from the `title` column using `lambda` and `.apply()`.
* Converted the `timeStamp` column from string to `DateTime` objects for easier time-based analysis.
* Created **new time-based columns**:

  * `Hour`
  * `Month`
  * `Day of Week` (mapped to actual day names)
  * `Date` (for time series analysis)

✅ **Analysis performed:**

* Identified **top 5 zip codes and townships** with the highest 911 call volumes.
* Checked **unique title codes** to understand the distribution of call types.
* Analyzed **the most common reasons for 911 calls**.

✅ **Visualization:**

* Created **count plots** using seaborn to visualize:

  * Distribution of calls by **Reason**
  * Calls by **Day of Week** with hue as Reason
  * Calls by **Month** with hue as Reason
* Used **line plots** to visualize:

  * Call volume trends across months (`lmplot`)
  * Daily call volumes over time
  * Separate time series for **EMS, Fire, and Traffic calls** to identify patterns.

✅ **Handled missing months in categorical plots** by using **line plots** to visualize call trends correctly.

✅ Used **legend adjustments and clear labeling** for professional, readable plots.

---

## 📊 Key Insights I Found

📌 **EMS calls are the most frequent reason** for 911 calls, followed by Traffic and Fire.

📌 **Weekdays have higher call volumes** than weekends for emergency calls.

📌 Clear **monthly trends** were observed using linear regression plots, showing seasonal patterns in emergency calls.

📌 Time series analysis revealed **specific spikes** on certain dates, useful for resource planning.

---

## 📌 What I Learned

✅ **Data cleaning and preparation** on real-world datasets

✅ **Feature extraction** using `.apply()` and `lambda` functions

✅ **Visual data analysis** using seaborn and matplotlib

✅ Understanding **temporal data patterns**

✅ How to handle missing values and interpret data insights systematically
