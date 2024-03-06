# CO2 Emission Dashboard

This Python script creates a dashboard for visualizing CO2 emissions and related data using Pandas, Panel, and HoloViews.

## Requirements

- Python 3.x
- [Poetry](https://python-poetry.org/)
- Pandas
- NumPy
- Panel
- HoloViews
- hvPlot

## Installation via poetry

the following command installs all necessary libraries listed in pyproject.toml
```bash
poetry isntall 
```

## Installation via pip

```bash
pip install pandas numpy panel holoviews hvplot
```

## Code level Usage

```python
# Import necessary libraries
import pandas as pd
import numpy as np
import panel as pn
pn.extension('tabulator')
import hvplot.pandas
from your_script_file import generate_dashboard

# Create an instance of the class
dashboard_generator = generate_dashboard()

# Generate and display the dashboard with export to HTML
dashboard_generator.generate(exportHTML=True)
```

## Usage via Poetry 

# Activate the virtual environment
poetry shell

# Run the script
python run python generatedashboard.py


- The script reads CO2 data from the [Our World in Data dataset](https://raw.githubusercontent.com/owid/co2-data/master/owid-co2-data.csv).
- The dashboard includes visualizations of CO2 emissions over time, CO2 vs. GDP scatterplot, and a bar chart of CO2 sources by continent.

To run the script, make sure you have the required dependencies installed and execute the code.

## License

This project is licensed under the [MIT License](LICENSE).
