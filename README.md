# regex

A simple command-line interface (CLI) tool for testing regular expressions in Python with visual feedback and pattern explanations.

## features
- Test regex patterns against arbitrary text
- Visual match highlighting in terminal output
- Interactive mode for live testing
- Automatic explanation of common regex components
- Clear visualization of match positions and counts

## installation
```shell script
# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install required package
pip install rich
```


## usage
### command line mode
```shell script
python regex.py -p "<pattern>" -t "<text>"
```


### interactive mode
```shell script
python regex.py --interactive
```


## example
Testing a pattern with command line arguments:
```shell script
python regex.py -p "\d{3}" -t "ABC123XYZ"
```


## key components
- `highlight_matches()`: Color-codes matches in terminal output
- `explain_pattern()`: Provides simple explanations for common regex elements
- `interactive_mode()`: Enables live testing with auto-refresh

## requirements
- Python 3.10+
- `rich` library (for enhanced terminal output)
