# Excel-Atlantic-Hurricanes-Dataset
Working with the Biggest Atlantic Hurricane dataset applying @switch' function


# Atlantic Hurricanes Dataset Analysis

## Overview
This project analyzes a dataset of the biggest Atlantic hurricanes and uses a switch function to categorize hurricanes based on their maximum wind speed. The goal is to classify hurricanes into categories (1 to 5) according to their wind speeds and output the results.

## Dataset
The dataset contains information about Atlantic hurricanes, including their names, dates, and maximum wind speeds. We focus on categorizing the hurricanes based on their maximum wind speed into five distinct categories.

## Hurricane Categories
The following categories are used to classify hurricanes based on their maximum wind speed (in mph):

# Define the categories as a dictionary
    category_map = {
        1: "Category 1: Winds 95-110 mph",
        2: "Category 2: Winds 110-129 mph",
        3: "Category 3: Winds 130-156 mph",
        4: "Category 4: Winds 157-180 mph",
        5: "Category 5: Winds 181+ mph"
    }
### Code Snippet
# Simulate the SWITCH logic using wind speed
    category = {
        wind_speed >= 157: 5,
        wind_speed >= 130: 4,
        wind_speed >= 111: 3,
        wind_speed >= 95: 2,
        wind_speed < 95: 1,
    }

    hurricane_category = category.get(True, "Unknown")  # default to "Unknown" if no category matches
    return category_map.get(hurricane_category, "Unknown")
