## Objectives

- Collect job data from the Jobs API
- Store the collected data in an Excel spreadsheet

## Files
| File | Description |
|------|-------------|
| `Jobs_API.ipynb` | Flask server that serves the jobs dataset as an API at `http://127.0.0.1:5000/data` |
| `Collecting_Jobs_data_Using_API.ipynb` | Client notebook that queries the API and collects job counts |
| `job-postings.xlsx` | Results: job postings by location and by technology |

## How it works
1. `Jobs_API` loads `jobs.json` and starts a Flask API.
2. The lab notebook sends GET requests with `requests`, filtering by `Key Skills` or `Location`.
3. The number of matching postings is counted and written to Excel with `openpyxl`.

## Sample results
| Query | Job postings |
|-------|-------------:|
| Python | 1173 |
| Los Angeles | 640 |

## Tools
Python · Flask · requests · pandas · openpyxl · IBM watsonx

