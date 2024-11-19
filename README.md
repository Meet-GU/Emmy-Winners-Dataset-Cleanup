# README

## Project Title: **IMDb Emmy Winners Data Scraper**

### Description:
This project is a Python-based script that retrieves data about Emmy-winning TV series from the IMDb API. The script uses the RapidAPI to access IMDb's API and fetches a list of Emmy-winning series, including various details such as title, ratings, release year, type, and more. The data is processed and cleaned, then saved into a CSV file for further analysis or usage.

### Requirements:
- Python 3.x
- Libraries: `pandas`, `numpy`, `requests`, `matplotlib`
  - Install the required libraries using pip:
    ```
    pip install pandas numpy requests matplotlib
    ```

### API Details:
This project interacts with the IMDb API using the RapidAPI platform.

- **API URL**: `https://imdb188.p.rapidapi.com/api/v1/emmyWinners`
- **RapidAPI Key**: `Your Key`

To use the API, you need to obtain your own API key from RapidAPI and replace the key in the script.

### How to Use:
1. Clone or download the repository.
2. Install the required libraries by running the following command:
   ```
   pip install -r requirements.txt
   ```
3. Run the script. It will send a GET request to the IMDb API and retrieve Emmy-winning series data.
4. The data is processed and cleaned in the script, then saved into a CSV file named `Series_details.csv`.

### Functionality:
- The script fetches a list of Emmy-winning series from the IMDb API.
- It extracts key information such as:
  - `id`: Unique identifier for each series.
  - `titleText`: Title of the series.
  - `Title_Type`: Type of the series (e.g., movie, series).
  - `topRanking`: Ranking of the series.
  - `Aggregate_Rating`: Overall rating of the series.
  - `Vote_Count`: Total number of votes.
  - `Release_Year`: Year of release.
  - `End_Year`: Year the series ended (if applicable).
  - `isAdult`: Whether the series is rated as adult content.
  - `is_Series`: Whether the entry is a series or episode.

- The data is cleaned by removing unnecessary columns and formatting the data types for proper analysis.
- The final DataFrame is saved as `Series_details.csv`.

### Example Output:
The final dataset, `Series_details.csv`, will contain the following columns:
- `id`: Series ID
- `titleText`: Title of the series
- `Title_Type`: Type of the series
- `topRanking`: Ranking of the series
- `Aggregate_Rating`: Overall rating
- `Vote_Count`: Number of votes
- `Release_Year`: Year of release
- `End_Year`: Year the series ended (if applicable)
- `isAdult`: Whether it's rated adult content
- `is_Series`: Whether it's a series or an episode

### Notes:
- Make sure to replace the RapidAPI key in the script before running it.
- The script processes data from the API, cleans it, and stores it into a CSV file for easy access and further analysis.

### License:
MIT License
