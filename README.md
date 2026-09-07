# regulex

A simple command-line interface (CLI) tool for testing regular expressions in Python with visual feedback and pattern explanations.

## Features
- Test regex patterns against arbitrary text
- Visual match highlighting in terminal output
- Interactive mode for live testing
- Automatic explanation of common regex components
- Clear visualization of match positions and counts

## Installation
```shell script
# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install required package
pip install rich
```


## Usage
### Command Line Mode
```shell script
python regulex.py -p "<pattern>" -t "<text>"
```


### Interactive Mode
```shell script
python regulex.py --interactive
```


## Example
Testing a pattern with command line arguments:
```shell script
python regulex.py -p "\d{3}" -t "ABC123XYZ"
```


## Key Components
- `highlight_matches()`: Color-codes matches in terminal output
- `explain_pattern()`: Provides simple explanations for common regex elements
- `interactive_mode()`: Enables live testing with auto-refresh

## Requirements
- Python 3.10+
- `rich` library (for enhanced terminal output)
