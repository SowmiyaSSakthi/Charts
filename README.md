# Sprint Data Visualization with Matplotlib and Pandas

A beginner-friendly Jupyter notebook that explores **12 chart types** in Python, using a small dataset of sprint metrics for three development teams. The same data is plotted in different ways to show how the choice of chart changes the story.

## Dataset

A small hand-made dataset built with a Pandas DataFrame (3 rows, 6 columns):

| Sprint | Task_completed | Bugs_reported | Hours_worked | Developers | Code_coverage |
|--------|----------------|---------------|--------------|------------|---------------|
| S1     | 25             | 1             | 230          | Team A     | 40            |
| S2     | 45             | 2             | 122          | Team B     | 70            |
| S3     | 78             | 6             | 320          | Team C     | 90            |

## Charts Covered

| # | Chart | Function | What it shows |
|---|-------|----------|---------------|
| 1 | Bar chart | `plt.bar()` | Tasks completed per sprint |
| 2 | Line plot | `plt.plot()` | Task progress across sprints |
| 3 | Pie chart | `plt.pie()` | Share of tasks completed by each team |
| 4 | Histogram | `plt.hist()` | Distribution of hours worked |
| 5 | Scatter plot | `plt.scatter()` | Hours worked vs. tasks completed |
| 6 | Box plot | `plt.boxplot()` | Spread of bugs reported |
| 7 | Horizontal bar chart | `plt.barh()` | Code coverage by team |
| 8 | Fill between | `plt.fill_between()` | Sprint progress as a filled area |
| 9 | Stack plot | `plt.stackplot()` | Tasks vs. bugs, stacked |
| 10 | Heatmap | `plt.imshow()` | All project metrics side by side |

## Getting Started

### Requirements

- Python 3.8+
- pandas
- matplotlib
- Jupyter Notebook, JupyterLab, or Google Colab




## Quick Example

```python
import pandas as pd
import matplotlib.pyplot as plt

data = {
    "Sprint": ["S1", "S2", "S3"],
    "Task_completed": [25, 45, 78],
    "Bugs_reported": [1, 2, 6],
    "Hours_worked": [230, 122, 320],
    "Developers": ["Team A", "Team B", "Team C"],
    "Code_coverage": [40, 70, 90],
}
df = pd.DataFrame(data)

plt.bar(df["Sprint"], df["Task_completed"])
plt.title("Tasks completed per sprint")
plt.xlabel("Sprint")
plt.ylabel("Tasks completed")
plt.show()
```

## Key Takeaways

- **Bar charts** make it easy to compare values across categories.
- **Line plots** show trends over time.
- **Scatter plots** reveal whether two variables are related, such as hours worked and output.
- **Heatmaps** give a compact overview of many metrics at once, though metrics with very different scales (hours vs. bugs) can dominate the color range.
- With only three data points, some charts (histogram, box plot) are for practice rather than real insight.

## Project Structure

```
.
├── Chart.ipynb             # Notebook with all charts
├── Chart_and_its_types.pdf # PDF export of the notebook
└── README.md
```

## Future Improvements

- [ ] Try a larger, real-world dataset
- [ ] Add Seaborn and Plotly versions of the charts
- [ ] Normalize metrics in the heatmap so scales are comparable
- [ ] Add subplots to compare charts side by side

