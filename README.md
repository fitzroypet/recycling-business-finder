# Recycling Business Finder

A Python application that uses Google Maps API to find and collect detailed information about recycling businesses across cities in the UK. The tool processes a CSV file containing city names and generates comprehensive JSON files containing business details including locations, operating hours, materials handled, and contact information.

## Project Structure

recycling-businesses/
├── city_20241119_055401.json # Example output data
├── recycling_business_finder.py # Main application script
└── requirements.txt # Project dependencies

ecycling-businesses/
├── data/
│ └── CityPopulation - Sheet1.csv # Input CSV file with city data
├── recyclers/ # Output directory for JSON files
│ └── city_name_YYYYMMDD_HHMMSS.json
├── recycling_business_finder.py # Main application script
└── requirements.txt # Project dependencies

## Features

- Search for recycling businesses in a specified location
- Collect detailed business information:
  - Name and address
  - Geographic coordinates
  - Contact details (phone, website)
  - Operating hours
  - Google ratings
  - Materials handled and recycling capabilities
  - Detailed address components
- Analyze business websites for additional recycling material information
- Export data to structured JSON format

## Prerequisites

- Python 3.x
- Google Maps API key
- Virtual environment (recommended)
- Required Python packages:
  - beautifulsoup4
  - googlemaps
  - requests
  - pandas
  - pyodbc
  - unixodbc

## Installation

1. Clone the repository:

bash
git clone https://github.com/fitzroypet/recycling-business-finder.git
<<<<<<< HEAD
cd recycling-business-finder
=======

cd recycling-businesses
>>>>>>> f89a424a0afdecdf2d16409c4b85ff31a6114f4b


2. Create and activate a virtual environment:

bash

python -m venv .venv


source .venv/bin/activate 


On Windows: .venv\Scripts\activate


3. Install required packages:

bash
pip install -r requirements.txt


## Usage

1. Prepare your data:
   - Place your city data CSV file in the `data` folder
   - Ensure the CSV has a "Built-up area" column containing city names

2. Replace the Google API key in `recycling_business_finder.py`:

python
GOOGLE_API_KEY = 'your_api_key_here'

3. Run the script:

bash
python recycling_business_finder.py

4. The script will:
   - Read cities from the CSV file
   - Search for recycling businesses in each city
   - Analyze each business's details and website
   - Generate JSON files in the `recyclers` folder

## Output

The script generates JSON files in the `recyclers` folder, with filenames following the pattern:
`city_name_YYYYMMDD_HHMMSS.json`

Each JSON file contains detailed information about unique recycling businesses found across all processed cities.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Author

Fitzroy Meyer-Petgrave

## Acknowledgments

- Google Maps Platform for providing location and business data
- Beautiful Soup for web scraping capabilities


