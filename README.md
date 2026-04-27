# PassGen

A simple, secure password generator written in Python.

## Features

- Generate strong, random passwords of configurable length
- Optionally include/exclude uppercase, lowercase, digits, and special characters
- Command-line interface for quick usage
- No dependencies beyond Python standard library
- Cross-platform

## Installation

```bash
pip install passgen
```

Or clone and install locally:

```bash
git clone https://github.com/<your-username>/passgen.git
cd passgen
pip install -e .
```

## Usage

```bash
passgen              # Generate a 16-character password with all character sets
passgen -l 20       # Generate a 20-character password
passgen -n          # Exclude special characters
passgen -d          # Exclude digits
passgen -l 10 -c    # Generate a 10-character password, only lowercase letters
```

Run `passgen --help` for full options.

## Development

### Requirements

- Python 3.8+

### Setup

```bash
python -m venv venv
source venv/bin/activate
pip install -e .[dev]
```

### Running Tests

```bash
pytest
```

### Building

```bash
python -m build
```

## License

MIT License - see the [LICENSE](LICENSE) file for details.
