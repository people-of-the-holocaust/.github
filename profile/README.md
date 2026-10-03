# People of the Holocaust

People of the Holocaust is a senior design project that transforms information from the United States Holocaust Memorial Museum's _Encyclopedia of Camps and Ghettos, 1933-1945_ into an accessible web-base database focused on individual people, places, and historical activity.

The project includes a Python interpreter/data pipeline for extracting structured data and a React frontend for browsing people, places, and map-based records.

## Live Site

[People of the Holocaust](people-of-the-holocaust.github.io/frontend)

## Project Purpose

The _Encyclopedia of Camps and Ghettos_ has a large amount of historical information, but is organized primarily around camps, ghettos, and locations. This project aims to reframe that information around individual people to aid researchers, students, and the public explore the human impact of the Holocaust.

## Team & Course Information

- University: Marquette University
- Course: Principles of Design - COSC 4920
- Team Members: Leyton Meadows, Danielle Idzi, Spencer O'Brien
- Advisors: Dr. Dennis Brylow (technical) & Dr. Peter Staudenmaier (historical)
- Project Duration: Fall 2025 - Present

## Features

- Searchable people database
- Searchable places database
- Interactive map view
- Python pipeline for extracting and structuring source data
- Static frontend deployable through GitHub Pages

## Repository Structure

```text
.
├── frontend/       # React/Vite web application
├── interpreter/    # Python data extraction and processing pipeline
├── documentation/  # Design documents, diagrams, presentations, and test plans
└── README.md       # Project overview
```

## Technology Stack

### Frontend

- React
- Vite
- React Router
- Leaflet
- PapaParse
- GitHub Pages

### Interpreter

- Python 3.11+
- pandas
- BeautifulSoup
- requests
- NLTK
- spaCy
- Supabase
- pytest

## Getting Started

### Frontend

```bash
cd frontend
npm install
npm run dev
```

Build for production:
`npm run build`

Preview the production build:
`npm run preview`

### Interpreter

```bash
cd interpreter
pip install .
my-tool
```

For development/testing:

```bash
cd interpreter
pip install -r requirements.txt
pytest
```

## Data Pipeline Overview

1. The interpreter processes source material from the _Encyclopedia of Camps and Ghettos_ by:
2. Loading known people and place data
3. Scraping article content
4. Splitting article text into sentences
5. Identifying sentences that mention known people
6. Extracting activities involving people and places
7. Writing structured activity records to CSV files or Supabase

## Documentation

Additional project materials are stored in `documentation/`, including:

- Software Design Document
- Test Plan
- Business Plan
- Final Presentation
- Database Schema
- Activity Diagram
- Data Structure Class Diagram

## Testing

Interpreter tests:

```bashj
cd interpreter
pytest
```

If frontend tests are added later, document them here.

## Deployment

The frontend is configured for GitHub Pages deployment:

```bash
cd frontend
npm run deploy
```

## Permissions and Sources

This project uses data derived from the United States Holocaust Memorial Museum's _Encyclopedia of Camps and Ghettos, 1933-1945_. Project and scraping permission documentation is stored in `documentation/`.
