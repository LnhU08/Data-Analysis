
# 📊 Udemy Course Dataset Report

## 📁 Dataset Information

This dataset contains information about over **3,600 courses** offered on Udemy, including key details such as price, number of subscribers, level, subject area, and publication time.

## 📌 Columns Description

| Column Name         | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `course_id`         | Unique identifier for each course                                           |
| `course_title`      | Title or name of the course                                                 |
| `is_paid`           | Whether the course is paid (`True`) or free (`False`)                       |
| `price`             | Price of the course (text format, converted to numeric in cleaned dataset)  |
| `num_subscribers`   | Number of users who enrolled in the course                                  |
| `num_reviews`       | Total number of user reviews                                                |
| `num_lectures`      | Number of video lectures in the course                                      |
| `level`             | Course difficulty level (Beginner, Intermediate, All Levels, etc.)          |
| `content_duration`  | Total duration of the course (e.g., "1.5 hours", "37 mins")                 |
| `subject`           | Subject area of the course (e.g., Business, Web Development, etc.)          |
| `published_timestamp` | Date and time when the course was published                             |
| `duration_hours`    | Converted duration in hours (from `content_duration`)                       |
| `year`              | Year extracted from `published_timestamp`                                   |
| `month`             | Month extracted from `published_timestamp`                                  |

## 🧹 Data Preprocessing Steps

The following transformations were applied to the original dataset:

1. **Price Cleanup**: Converted text-based prices (e.g., "$75", "Free") to numeric values.
2. **Duration Conversion**: Converted `content_duration` into numeric `duration_hours`.
3. **Datetime Parsing**: Extracted `year` and `month` from the course `published_timestamp`.

The cleaned dataset is saved as `cleaned_dataset.csv`.

## 📈 Dashboard Metrics (in Excel)

You can use the cleaned dataset to build a visual dashboard using Excel with the following insights:

- 📌 Total Courses, Total Subscribers, Average Course Duration
- 📚 Course distribution by **subject** and **level**
- 💵 Revenue potential analysis (Paid vs Free)
- 📊 Trend of course publication by year/month
- 🎯 Top subjects with highest number of subscribers or reviews

## 🔧 Tools Used

- **Python (Pandas)** for data cleaning
- **Excel** for visualization and dashboard creation

## 📂 Files

- `dataset.csv`: Original raw dataset
- `cleaned_dataset.csv`: Cleaned and ready-to-analyze dataset
