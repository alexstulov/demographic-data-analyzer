# Demographic data analyzer

Analyze demographic data using Pandas.  

## How to use
To run sample code and tests go to `src` folder and start `main.py` with `python` command:

```bash
cd ./src
python main.py
```

## Data
Demographic data was extracted from the 1994 Census database. Sample of the data:

|    | age        | workclass | fnlwgt | education  | education-num | ... | capital-gain | capital-loss | hours-per-week | native-country | salary |
| ---|------------| --------- | ------: | ---------- | -------------: | --- | ------------: | ------------: | --------------: | -------------- | ------: |
| 0  | 39         | State-gov | 77516 | Bachelors   | 13 | ... | 2174 | 0 | 40 | United-States | <=50K
| 1  | 50         | Self-emp-not-inc | 83311 | Bachelors | 13 | ... | 0 | 0 | 13 | United-States | <=50K
| 2  | 38         | Private | 215646   | HS-grad         | 9 | ... | 0 | 0 | 40 | United-States | <=50K
| 3  | 53         | Private | 234721      | 11th         | 7 | ... | 0 | 0 | 40 | United-States | <=50K
| 4  | 28         | Private | 338409  | Bachelors        | 13 | ... | 0 | 0 | 40 | Cuba | <=50K

[5 rows x 15 columns]

## What the app does
Analyzer answers following questions:

* How many people of each race are represented in this dataset? This * should be a Pandas series with race names as the index labels. (race * column)
* What is the average age of men?
* What is the percentage of people who have a Bachelor's degree?
* What percentage of people with advanced education (Bachelors, Masters, * or Doctorate) make more than 50K?
* What percentage of people without advanced education make more than 50K?
* What is the minimum number of hours a person works per week?
* What percentage of the people who work the minimum number of hours per * week have a salary of more than 50K?
* What country has the highest percentage of people that earn >50K and * what is that percentage?
* Identify the most popular occupation for those who earn >50K in India.

## Results

### Number of each race:
| race | count |
| ----------------- | ---: |
| Amer-Indian-Eskimo     | 311|
| Asian-Pac-Islander     | 1039|
| Black                  | 3124|
| Other                   | 271|
| White                 | 27816|

### Theses:
* Average age of men: 39.4,
* Percentage with Bachelors degrees: 16.4%,
* Percentage with higher education, that earn >50K: 46.5%,
* Percentage without higher education, that earn >50K: 17.4%,
* Minimum work time: 1 hour/week,
* Percentage of rich among those, who work fewest hours: 10.0%,
* Country with highest percentage of rich: Iran,
* Highest percentage of rich people in country: 41.9%,
* Top occupations in India: Prof-specialty.