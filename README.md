# Health SQL Analysis

This repository contains SQL queries designed to analyze health-related datasets.
The goal is to demonstrate practical SQL skills in a healthcare and biotech context.

## Dataset

The dataset simulates patient health records including:
- Age
- Gender
- Cholesterol level
- Blood pressure

## Key Questions Answered

- What is the average cholesterol level by age group?
- Which patients fall into a high-risk category?
- Are there differences between genders?
- How can simple JOIN operations be used in healthcare data?

## Sample SQL Queries

```sql
-- Average cholesterol by age group
SELECT
  CASE
    WHEN age < 30 THEN 'Under 30'
    WHEN age BETWEEN 30 AND 45 THEN '30-45'
    ELSE '46+'
  END AS age_group,
  AVG(cholesterol) AS avg_cholesterol
FROM patients
GROUP BY age_group;

Commit message:

---

## 4️⃣ Dataset ekle.

Repo ana sayfa → **Add file → Create new file**

Dosya adı:
