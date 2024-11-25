# XXE File Upload Tester

A Flask-based web-ui that allows user to create XLSX and DOCX documents to test XXE on file upload endpoints.
Web-UI also has a feature to test your created document if it is abusing vulnerable parser properly or not.

## Prerequisites

- Python 3.x
- Virtual environment (recommended)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/divinepwner/XXE-OOB-Helper.git
cd XXE-OOB-Helper
```

2. Create and activate virtual environment:
```bash
python -m venv venv
source venv/bin/activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Dependencies

The following packages are required and included in requirements.txt:
- Flask
- python-docx
- openpyxl
- requests
- lxml

## Usage

1. Start the server:
```bash
python3 app.py
```

The tool will be up on `http://localhost:5000`

## Development

To modify the port or host, edit `app.py`:
```python
if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000)
```
