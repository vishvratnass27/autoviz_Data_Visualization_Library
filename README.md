
# AutoViz: Automated Visualization for Data Exploration

AutoViz is a Python library that simplifies the process of data exploration and visualization. It automatically generates a variety of informative charts and graphs to help you understand your dataset quickly. In this readme, we will walk you through an example of using AutoViz to visualize a dataset.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Example](#example)
- [Documentation](#documentation)
- [Contributing](#contributing)
- [License](#license)

## Installation

To use AutoViz, you first need to install it via pip:

```bash
pip install autoviz
```

## Usage

AutoViz is a powerful tool for data visualization, and you can use it in various scenarios. Here's a simple example of how to use AutoViz to visualize a dataset:

```python
from autoviz.AutoViz_Class import AutoViz_Class

# Initialize AutoViz
AV = AutoViz_Class()

# Load your dataset
filename = "train.csv"

# Specify the separator used in your dataset (e.g., comma)
sep = ","

# Perform automatic visualization
dft = AV.AutoViz(
    filename,
    sep=sep,
    depVar="",
    dfte=None,
    header=0,
    verbose=0,
    lowess=False,
    chart_format="svg",
    max_rows_analyzed=150000,
    max_cols_analyzed=30,
)
```

In this code snippet, we import AutoViz, initialize it, and then use it to automatically visualize the dataset in the "train.csv" file.

## Example

Let's break down the parameters used in the `AutoViz` function:

- `filename`: The name of the dataset file you want to visualize.
- `sep`: The separator used in your dataset, such as a comma.
- `depVar`: The dependent variable, which is useful for regression analysis (leave it empty for exploratory visualization).
- `dfte`: A test dataset (leave it as None for this example).
- `header`: The row number that contains the column names (0 in this case).
- `verbose`: Set to 0 for minimal output.
- `lowess`: Set to False to disable the LOWESS smoothing.
- `chart_format`: The format for saving the charts (SVG in this example).
- `max_rows_analyzed`: The maximum number of rows to analyze.
- `max_cols_analyzed`: The maximum number of columns to analyze.

With these parameters set, AutoViz will generate various charts and graphs to help you explore and understand your dataset.

## Documentation

For more detailed information on AutoViz and its capabilities, refer to the official documentation: [AutoViz Documentation](https://github.com/AutoViML/AutoViz).

---

That's it! You now have a basic understanding of how to use AutoViz for automated data visualization. Feel free to explore the library further and adapt it to your specific data exploration needs. If you encounter any issues or have questions, don't hesitate to reach out to the AutoViz community on GitHub.
