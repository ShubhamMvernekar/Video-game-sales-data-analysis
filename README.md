
# Video Game Sales Data Analysis

This repository contains a detailed analysis of a video game sales dataset using various data analysis and visualization techniques. The dataset includes information on video game sales, including attributes such as genre, platform, year of release, publisher, and sales figures across different regions.

## Project Overview

The project aims to explore and analyze video game sales data to uncover patterns and insights related to game popularity, sales trends, and market performance. The primary focus areas include:
- Visualizing sales trends by year, platform, and genre.
- Investigating the relationship between sales and game attributes (e.g., genre, platform, publisher).
- Performing exploratory data analysis (EDA) to identify key insights and outliers.

## Dataset

The dataset used for this analysis is sourced from Kaggle (or a similar platform), which contains sales data for video games over the years. The dataset has the following key columns:
- `Name`: The title of the game.
- `Platform`: The gaming platform (e.g., PS4, Xbox One, etc.).
- `Year_of_Release`: The year the game was released.
- `Genre`: The genre of the game (e.g., action, adventure, etc.).
- `Publisher`: The publisher of the game.
- `NA_Sales`: Sales in North America (in millions).
- `EU_Sales`: Sales in Europe (in millions).
- `JP_Sales`: Sales in Japan (in millions).
- `Other_Sales`: Sales in other regions (in millions).
- `Global_Sales`: Total worldwide sales (in millions).

## Tools & Technologies

- **Python**: The primary programming language used for data analysis.
- **Pandas**: For data manipulation and analysis.
- **Matplotlib & Seaborn**: For data visualization and plotting.
- **Jupyter Notebooks**: For an interactive analysis environment.

## Installation

To get started with this project, you need to have Python installed on your system. Follow these steps to set up the environment:

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/ShubhamMvernekar/Video-game-sales-data-analysis.git
   cd Video-game-sales-data-analysis
   ```

2. Install the required dependencies using `pip`:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Open the analysis notebooks to explore the data.

## Project Structure

- `data/`: Contains the raw dataset used for analysis.
- `notebooks/`: Jupyter notebooks with data analysis and visualizations.
- `requirements.txt`: A list of dependencies required to run the project.
- `README.md`: This file.

## Key Insights

1. **Sales Trends Over Time**: Visualizations showing how video game sales have changed over the years, including peaks during certain periods.
2. **Platform Popularity**: Analysis of the most successful platforms based on global sales.
3. **Genre Breakdown**: Exploration of which genres perform best in terms of sales across different regions.
4. **Publisher Performance**: Insights into the top-performing video game publishers.

## Usage

Once the environment is set up, you can open the Jupyter notebooks to run the analyses. You can customize and extend the analysis by adding new visualizations, exploring other patterns, or incorporating new data sources.

### Example Usage

```python
import pandas as pd
import matplotlib.pyplot as plt

# Load the dataset
df = pd.read_csv('data/vgsales.csv')

# Analyze the top 10 best-selling games globally
top_10_games = df.nlargest(10, 'Global_Sales')

# Plot the top 10 games
top_10_games.plot(kind='bar', x='Name', y='Global_Sales', title="Top 10 Best Selling Games", legend=False)
plt.ylabel('Global Sales (millions)')
plt.show()
```

## Contributing

Feel free to fork the repository, make improvements, or suggest changes. If you'd like to contribute, please open an issue or submit a pull request.

## License

This project is open-source and available under the [MIT License](LICENSE).
