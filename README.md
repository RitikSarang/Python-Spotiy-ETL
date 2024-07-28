# Spotify Data Extraction

This repository contains a Python script for extracting and analyzing data from the Spotify API. The script retrieves information about songs, albums, artists, and playlists, processes this data, and saves it into CSV files for further analysis.

## Overview

The script performs the following tasks:

1. **Authentication**: Uses Spotify API credentials to access the Spotify Web API.
2. **Data Extraction**: Retrieves details from a specified Spotify playlist, including song names, album types, release dates, and more.
3. **Data Processing**: Converts raw data into structured DataFrames.
4. **Data Export**: Saves the processed data into CSV files.

## Table of Contents

- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Data Structure](#data-structure)

## Requirements

Ensure you have Python installed on your system. The script requires the following Python packages:

- `spotipy`: For interacting with the Spotify Web API
- `pandas`: For data manipulation and analysis
- `json`: For handling JSON data
- `datetime`: For managing date and time

You can install the necessary packages using pip:

```bash
pip install spotipy pandas
```
## Installation

Set Up API Credentials

Create a credet_YYYY-MM-DD.json file in the Data engineering/Python/Day 1/ directory with your Spotify API credentials. The file should contain:

```bash
{
    "client_id": "YOUR_CLIENT_ID",
    "client_secret": "YOUR_CLIENT_SECRET"
}
```

## Usage

This script will:

- `Authenticate with Spotify using your API credentials.`
- `Extract data from a specified playlist.`
- `Process the data into DataFrames.`
- `Save the data into CSV files named Spotiy_data_YYYY-MM-DD.csv and Spotiy_artist_data_YYYY-MM-DD.csv.`

Check Output Files:

- `Spotiy_data_YYYY-MM-DD.csv: Contains information about the songs in the playlist, including song names, release dates, popularity, and more.`
- `Spotiy_artist_data_YYYY-MM-DD.csv: Contains details about the artists, including their IDs, names, types, and external URLs.`

## Data Structure
Song Data (Spotiy_data_YYYY-MM-DD.csv)
![image](https://github.com/user-attachments/assets/8737adcc-ebd6-4889-9219-2054c1709d76)

Artist Data (Spotiy_artist_data_YYYY-MM-DD.csv)
![image](https://github.com/user-attachments/assets/4537addd-bfd5-4736-bfda-2ee53d637d75)
