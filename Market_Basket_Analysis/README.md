# Market Basket Analysis using Apriori Algorithm

## Overview

This project demonstrates Market Basket Analysis using the Apriori algorithm on a synthetic transactional dataset of student stationery purchases. The objective is to discover frequently occurring item combinations and generate association rules that reveal relationships between stationery products.

The project applies association rule mining techniques to identify purchasing patterns using support, confidence, and lift metrics. Visualizations are used to analyze the strength and significance of the generated rules.

---

## Dataset

A synthetic dataset containing 1000 transactions was created to simulate stationery purchases. Each transaction consists of combinations of items such as:

* Notebook
* Pen
* Pencil
* Eraser
* Sharpener
* Geometry Box
* Calculator
* Highlighter
* Sticky Notes
* File Folder

Several realistic purchasing patterns were intentionally incorporated into the dataset, such as:

* Notebook → Pen
* Pencil → Eraser
* Geometry Box → Calculator
* Notebook → Highlighter

These patterns allow the Apriori algorithm to discover meaningful associations between products.

---

## Project Workflow

1. Generate a synthetic transactional dataset.
2. Perform exploratory data analysis (EDA).
3. Convert transactions into one-hot encoded format.
4. Apply the Apriori algorithm to identify frequent itemsets.
5. Generate association rules using support, confidence, and lift.
6. Visualize association rules using scatter plots.
7. Filter and interpret meaningful rules.
8. Discuss ethical considerations.

---

## Exploratory Data Analysis

The following analyses were performed:

* Item frequency distribution
* Transaction-level inspection
* Identification of popular stationery products

---

## Apriori Algorithm

The Apriori algorithm was applied with a minimum support threshold of 0.03 to identify frequent itemsets.

Association rules were then generated and evaluated using:

* Support
* Confidence
* Lift

---

## Visualizations

### Item Frequency Distribution

Shows the popularity of stationery items across all transactions.

### Support vs Confidence Plot

Visualizes the relationship between support and confidence for generated association rules.

### Lift vs Confidence Plot

Highlights the strength of associations and helps identify the most valuable rules.

---

## Key Findings

* Notebooks, pencils, and pens appeared among the most frequent items.
* Strong associations were observed between notebooks and pens.
* Pencil-related purchases frequently included erasers.
* Geometry boxes and calculators formed meaningful item combinations.
* Several association rules achieved high lift values, indicating strong relationships between products.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Mlxtend
* Jupyter Notebook

---

## Ethical Considerations

Since the dataset is synthetic and does not contain personal information, there are no direct privacy concerns. However, the project discusses potential biases, misuse of association rules, and responsible use of recommendation systems.

---

## Conclusion

This project demonstrates how the Apriori algorithm can be used to discover meaningful relationships within transactional data. The generated association rules provide insights into common stationery purchase patterns and illustrate the practical application of association rule mining techniques.

---

## Author

Rajat Kumar <br>

Professional Master's in Data Science and AI <br>
Master of Science in Mathematics

