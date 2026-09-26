# JobCruncher

JobCruncher is a Flask application that collects public job listings, stores them in MongoDB, and provides a browser interface for searching and filtering recent opportunities.

This repository is my contribution fork of [TejasPrabhu/Job-Analyzer](https://github.com/TejasPrabhu/Job-Analyzer).

## My contributions

My work included:

- Extending scraper behavior and custom URL handling
- Adding MongoDB setup and continuous-integration support
- Expanding Flask and scraper tests
- Improving code coverage and fixing test failures
- Documenting installation and the project structure
- Adding screenshots, project context, and a future roadmap

## Technology

- Python
- Flask
- MongoDB
- Selenium
- Pytest
- GitHub Actions

## Repository structure

```text
src/        Flask application and scraper
test/       Flask and scraper tests
data/       Sample and generated data
docs/       Project documentation
```

## Local setup

Create a virtual environment and install the dependencies:

```bash
python -m venv .venv
```

On Windows:

```powershell
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

On Linux or macOS:

```bash
source .venv/bin/activate
pip install -r requirements.txt
```

Start MongoDB, configure the application for your local instance, and then run:

```bash
cd src
flask --app app run --debug
```

The scraper depends on Selenium and on the current structure and policies of third-party sites. Review the target site's terms and update selectors before using it.

## Testing

```bash
pytest
```

## What I learned

- How to test Flask routes and scraper behavior
- How to connect a data-collection task to MongoDB and a web interface
- How continuous integration exposes environment assumptions
- Why web scrapers need maintenance, rate limits, and responsible data practices

## Status

This is an archived course project and contribution fork. Dependencies and scraper selectors are dated and should be upgraded before reuse.

## License

This project is available under the license included in the repository. Credit for the original project and other contributions belongs to the upstream maintainers and contributors.

