# Exploring NYC Public School Test Result Scores

This project analyzes standardized test performance data from New York City's public schools to identify schools with top math results, examine performance variations by borough, and determine the city's top ten performing schools based on combined SAT scores.

## Project Description

Every year, school test results impact the college admissions fate of millions of students. This analysis focuses on:

1. **Identifying schools with the best math results**:
   - Schools where the average math score is at least 80% of the maximum possible score (640 out of 800).
   - Results are saved in a DataFrame called `best_math_schools`, including `school_name` and `average_math`, sorted in descending order.
<br>
2. **Finding the top 10 performing schools based on combined SAT scores**:
   - Calculating `total_SAT` as the sum of math, reading, and writing scores.
   - Results are saved in a DataFrame called `top_10_schools`, including `school_name` and `total_SAT`, sorted in descending order.
<br>
3. **Determining which borough has the largest standard deviation in combined SAT scores**:
   - Analyzing variability to identify disparities within boroughs.
   - Results are saved in a DataFrame called `largest_std_dev`, including `borough`, `num_schools`, `average_SAT`, and `std_SAT`, rounded to two decimal places.

## Dataset

The dataset used is `schools.csv`, which contains information on NYC public schools, including:

- School names
- Boroughs
- Average scores for math, reading, and writing

## Requirements

- Python 3.x
- pandas library

## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   ```

2. **Navigate to the project directory**:

   ```bash
   cd your-repo-name
   ```

3. **Install the required packages**:

   ```bash
   pip install pandas
   ```

## Results

### 1. Best Math Results
- **Criteria**: Schools with average math scores of at least 640 (80% of the maximum score of 800).
- **Top Schools**:
  | Rank | School Name                                                             | Average Math |
  |------|------------------------------------------------------------------------|--------------|
  | 1    | Stuyvesant High School                                                | 754          |
  | 2    | Bronx High School of Science                                          | 714          |
  | 3    | Staten Island Technical High School                                   | 711          |
  | 4    | Queens High School for the Sciences at York College                   | 701          |
  | 5    | High School for Mathematics, Science, and Engineering at City College | 683          |

### 2. Top 10 Performing Schools (Combined SAT Scores)
- **Criteria**: Schools ranked by `total_SAT`, the sum of average math, reading, and writing scores.
- **Top Schools**:
  | Rank | School Name                                                             | Total SAT |
  |------|------------------------------------------------------------------------|-----------|
  | 1    | Stuyvesant High School                                                | 2144      |
  | 2    | Bronx High School of Science                                          | 2041      |
  | 3    | Staten Island Technical High School                                   | 2041      |
  | 4    | High School of American Studies at Lehman College                     | 2013      |
  | 5    | Townsend Harris High School                                           | 1981      |
  | 6    | Queens High School for the Sciences at York College                   | 1947      |
  | 7    | Bard High School Early College                                        | 1914      |
  | 8    | Brooklyn Technical High School                                        | 1896      |
  | 9    | Eleanor Roosevelt High School                                         | 1889      |
  | 10   | High School for Mathematics, Science, and Engineering at City College | 1889      |

### 3. Borough with the Largest Standard Deviation in SAT Scores
- **Criteria**: The borough with the highest variability in SAT performance.
- **Result**: Manhattan

Manhattan had the highest standard deviation in combined SAT scores, reflecting greater variability in student performance across its schools.

## License

This project is licensed under the MIT License.