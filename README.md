# Cable & Busbar Sizing Tool

This project provides a small in‑browser utility for selecting suitable cable and busbar sizes based on Indian Standard (IS) data. The tool is built entirely in HTML, CSS and JavaScript so it can be run without any server.

## Setup

1. Clone or download this repository.
2. No extra build steps are required – all logic lives in `index.html`, `app.js` and `styles.css`.
3. Open `index.html` in any modern web browser (for example by double clicking it).

## Usage

1. Choose whether you wish to size a cable or a busbar.
2. Fill in system parameters such as voltage, load current or power, conductor material and installation method.
3. Click **Calculate** to display the sizing results. You can download the calculated data as CSV or save your current configuration as a JSON file.
4. To load a previously saved configuration, use the **Load Configuration & Calculate** button at the top of the page. Select your JSON file and the form will populate and immediately run the calculation.

## Data Sources

The data used by this tool was extracted from the following Bureau of Indian Standards publications, included in the `standards/` directory:

- **IS 3961 (Part 2):2017**
- **IS 3961 (Part 6)**
- **IS 8623 (Part 1):1993**
- **IS 8623 (Part 2):1993**

Relevant tables from these documents have been compiled into `data/IS_standard_sizing_data.json` for use by the application.

The PDFs themselves remain the property of the Bureau of Indian Standards (BIS) and are provided here for reference only. Please ensure you comply with any applicable copyright or licensing requirements when using these files.

## Running Locally

Simply open `index.html` in your browser. Everything executes locally with no dependencies. If you prefer to serve the files via a lightweight web server (for example when testing on mobile devices), any static file server will work.

## License

No explicit software license has been provided with this project. If you plan to use the IS standards data or PDFs commercially or distribute them further, consult the BIS terms of use.
