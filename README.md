# Vanguard Interface A/B Analysis

## Project Overview

This project analyzes the impact of a new user interface design for Vanguard’s platform. The goal is to evaluate whether the new design improves user engagement, completion rates, and process efficiency compared to the traditional interface.

The analysis focuses on metrics such as completion rate, time spent per step, error rates, and demographic influences. Statistical tests were performed to assess the significance of observed differences.

---

## Data Description

The dataset contains anonymized data on Vanguard customers interacting with the platform under two different UI designs:

* **Control Group:** Users with the traditional interface.
* **Test Group:** Users with the new interface.

**Key variables include:**

* `id_cliente`: Customer identifier
* `modalidad`: Process group (Test or Control)
* `paso_proceso`: Step in the process (start, step 1, step 2, confirm, etc.)
* `meses_permanencia`: Customer tenure
* `edad`: Customer age
* `genero`: Customer gender
* Metrics such as session duration, errors (backtracking), and completion.

---

## Analysis

The project involves:

1. **Descriptive statistics**

   * Completion rates per group
   * Time spent per step
   * Error rates

2. **Statistical testing**

   * **Completion rate:** Z-test to compare Test vs Control
   * **Tenure:** t-test for equality of means
   * **Age and Gender:** Chi-square test for group differences

3. **Evaluation of process performance**

   * Identify bottlenecks and steps where users struggle
   * Compare efficiency of new vs old interface

---

## Key Findings

* **Completion Rate:**

  * Control: 65.54%
  * Test: 69.26%
  * Z = 29.221, p-value = 0.0 → Statistically significant difference
  * However, the increase (3%) does **not meet Vanguard’s 5% threshold** for cost-effectiveness.

* **Time Spent per Step:**

  * Overall process duration is similar between groups
  * Test group is slightly faster except for start and step 2

* **Error Rate:**

  * Overall error rate: 8.05%
  * Control: 6.70%, Test: 9.14%
  * Backtracking indicates small increases in Test group

* **Demographics:**

  * Age differs significantly between groups
  * Tenure is similar → differences in completion or errors are due to UI design, not customer experience
  * Gender distribution shows significant differences

* **Bias & Limitations:**

  * Test group is slightly younger
  * Experiment not perfectly randomized
  * Observed performance differences may be partially influenced by age and gender

---

## Requirements

* Python 3.10+
* Jupyter Notebook or any Python IDE
* Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`, `statsmodels`

---

## Usage

1. Clone the repository:

```bash
git clone https://github.com/tu_usuario/vanguard_ab_analysis.git
```

2. Install required packages:

```bash
pip install -r requirements.txt
```

3. Run the analysis notebook or script:

```bash
jupyter notebook proyect5.ipynb
# or
python proyect5.py
```

---

## Conclusion

The new UI design increases the completion rate and improves process efficiency in some steps.
Although the improvement is statistically significant, the increase does not reach the 5% threshold required by Vanguard for justifying implementation costs.

Future analysis could include:

* Broader demographic and usage data
* Device/browser information
* Conversion or revenue metrics

---

## Author
Javier Soto Gonzalez | javisoto2001@gmail.com | https://github.com/javiersoto16
Ignacio Sabatell Lopez  |  ignaciosabatel@gmail.com  |  https://github.com/ignaciosabatell


