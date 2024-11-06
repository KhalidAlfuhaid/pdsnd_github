<!-- >**Note**: Please **fork** the current Udacity repository so that you will have a **remote** repository in **your** Github account. Clone the remote repository to your local machine. Later, as a part of the project "Post your Work on Github", you will push your proposed changes to the remote repository in your Github account.

### Date created
Include the date you created this project and README file.

### Project Title
Replace the Project Title

### Description
Describe what your project is about and what it does

### Files used
Include the files used

### Credits
It's important to give proper credit. Add links to any repo that inspired you or blogposts you consulted.
 -->

# US Bikeshare Data Analysis Program

## Description

This Python program analyzes bike sharing system data from three major US cities: Chicago, New York City, and Washington. It provides an interactive way to explore bike share usage patterns by filtering data based on city, month, and day of the week.

## Features

- Filter bike share data by:
  - City (Chicago, New York City, Washington)
  - Month (January through June)
  - Day of the week
- View various statistics including:
  - Most popular times of travel
  - Most popular stations and trips
  - Trip duration information
  - User demographics

## Requirements

- Python 3.x
- pandas
- numpy

## Dependencies Installation

```bash
pip install pandas numpy
```

## Required Files

The program expects the following CSV files in the same directory:

- chicago.csv
- new_york_city.csv
- washington.csv

## Usage

1. Run the program:

```bash
python bikeshare.py
```

2. Follow the interactive prompts to:

   - Select a city
   - Choose a month for filtering (or 'all')
   - Select a day of the week (or 'all')

3. View the analysis results

4. Choose whether to restart the analysis with different filters

## Program Structure

### Main Functions

#### `get_filters()`

- Handles user input for city, month, and day selections
- Implements input validation
- Returns selected filters

#### `load_data(city, month, day)`

- Loads data from the appropriate CSV file
- Applies time filters based on user selection
- Returns filtered DataFrame

#### `time_stats(df)`

- Calculates most frequent times of travel
- Shows popular months, days, and hours

#### `station_stats(df)`

- Identifies most popular stations and trip routes
- Analyzes start and end station combinations

#### `trip_duration_stats(df)`

- Calculates total and average trip durations
- Provides time-based analysis

#### `user_stats(df)`

- Analyzes user demographics
- Shows breakdowns by user type and gender
- Provides age statistics based on birth year

## Data Structure

The program expects CSV files with the following columns:

- Start Time
- End Time
- Trip Duration
- Start Station
- End Station
- User Type
- Additional demographic data (varies by city)

## Error Handling

- The program includes input validation for city, month, and day selections
- Handles missing data gracefully
- Provides appropriate error messages for invalid inputs

## Contributing

To contribute to this project:

1. Fork the repository
2. Create a new branch for your feature
3. Commit your changes
4. Push to your branch
5. Create a Pull Request

## License

This project is available for public use. Please provide attribution when using or modifying the code.
