# Recycling Business Finder

A Python application that uses Google Maps API to find and collect detailed information about recycling businesses in a specified location. The tool generates a comprehensive JSON file containing business details including locations, operating hours, materials handled, and contact information.

## Project Structure

recycling-businesses/
├── middlesbrough_UK_20241119_055401.json # Example output data
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
  - pyodbc
  - unixodbc

## Installation

1. Clone the repository:

bash
git clone https://github.com/yourusername/recycling-businesses.git
cd recycling-businesses


2. Create and activate a virtual environment:

bash
python -m venv .venv
source .venv/bin/activate # On Windows: .venv\Scripts\activate


3. Install required packages:

bash
pip install -r requirements.txt


## Usage

1. Replace the Google API key in `recycling_business_finder.py`:

python
GOOGLE_API_KEY = 'your_api_key_here'

2. Run the script:

bash
python recycling_business_finder.py


3. When prompted, enter a location (e.g., "Middlesbrough, UK")

4. The script will:
   - Search for recycling businesses in the specified location
   - Analyze each business's details and website
   - Generate a JSON file with the collected data

## Output

The script generates a JSON file using a combination of the city, country, date, and time (e.g., `middlesbrough_UK_20241119_055401.json`) containing detailed information about each recycling business found in the specified location.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Author

Fitzroy Petgrave

## Acknowledgments

- Google Maps Platform for providing location and business data
- Beautiful Soup for web scraping capabilities


