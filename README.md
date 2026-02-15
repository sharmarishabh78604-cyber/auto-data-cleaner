# Auto Data Cleaner Website

A lightweight Python web app that cleans, sorts, deduplicates, and stores raw datasets provided in JSON or CSV format.

---

## Features

* Cleans field names (trims spaces, lowercase, underscores)
* Cleans values (removes extra spaces)
* Removes duplicate rows
* Sorts by selected field
* Stores cleaned datasets in SQLite
* View dataset history

---

## Tech Stack

* Python (built-in HTTP server)
* SQLite
* HTML + CSS

No external dependencies required.

---

## Project Structure

```
auto-data-cleaner/
│
├── app.py
├── requirements.txt
├── README.md
│
├── static/
│   └── style.css
│
└── tests/
    └── test_app.py
```

---

## Run Locally

```bash
python3 app.py
```

Open browser:

```
http://localhost:5000
```

---

## Input Examples

### JSON

```json
[
  {"Name": " Ana ", "Age": 22},
  {"Name": "zoe", "Age": 20},
  {"Name": "Ana", "Age": 22}
]
```

### CSV

```csv
Name,Age
 Ana ,22
zoe,20
Ana,22
```

---

## Run Tests

```bash
python3 -m unittest discover tests
```

---

## License

Free to use for learning and projects.
