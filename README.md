# TrendTags - Tag Generator

[![Python Lint](https://github.com/imDarshanGK/TrendTags/actions/workflows/python-lint.yml/badge.svg)](https://github.com/imDarshanGK/TrendTags/actions)
[![JS Lint](https://github.com/imDarshanGK/TrendTags/actions/workflows/js-lint.yml/badge.svg)](https://github.com/imDarshanGK/TrendTags/actions)
[![CodeQL](https://github.com/imDarshanGK/TrendTags/actions/workflows/codeql.yml/badge.svg)](https://github.com/imDarshanGK/TrendTags/actions)

## Features

- Real-time tag generation from YouTube trends
- One-click copy all tags
- Clean responsive interface
- Fast Flask-powered backend
- Auto-updating tag database

## Installation 🛠️

### Prerequisites

- Python >=3.12
- YouTube API key

### Quick Start

1. Clone the repository and navigate to it in the command line:

    ```bash
    git clone https://github.com/your-username/TrendTags.git
    cd TrendTags
    ```

2. Create `.env` file:

    ```bash
    cp .env.example .env
    nano .env  # Add your actual API keys
    ```

    Then edit `.env` and replace placeholder values:

    ```env
    # SECURITY WARNING!
    # 1. Rename this to .env
    # 2. Never commit real keys
    # 3. Get keys from Google Cloud Console

    YOUTUBE_API_KEY=your_key_here
    RAPIDAPI_KEY=your_key_here
    ```

3. Set up environment:

    ```bash
    pip install -r requirements.txt
    ```

4. Run the application:

    ```bash
    python app.py
    ```

## Usage

1. Enter your video topic (e.g., "cooking", "tech reviews")
2. Select number of tags (10-30)
3. Click "Generate Tags"
4. Copy tags with one click

## Project Structure

```bash
TrendTags/
├── .github/           # CI/CD workflows
│   └── workflows/     # GitHub Actions
├── static/            # Frontend assets
│   ├── css/           # Stylesheets
│   └── js/            # JavaScript
├── templates/         # HTML templates
├── tests/             # Pytest tests
├── src/               # Source code
│   ├── config.py      # Configuration
│   └── ...            # Other modules
├── app.py             # Main application
├── requirements.txt   # Dependencies
├── LICENSE            # MIT License
└── README.md          # This file
```

## Code Quality

To check Python code style and run tests:

```bash
flake8 src tests app.py
black --check src tests app.py
pytest
```

To check JavaScript code style:

```bash
npx eslint static/js
npx prettier --check static/js
```

## Contributing

We welcome contributions! Please see our [CONTRIBUTING.md](CONTRIBUTING.md) for:

- How to report issues
- Code style guidelines
- Pull request process
- Commit message standards

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.