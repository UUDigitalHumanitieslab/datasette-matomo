# datasette-matomo

[![PyPI](https://img.shields.io/pypi/v/datasette-matomo.svg)](https://pypi.org/project/datasette-matomo/)
[![Changelog](https://img.shields.io/github/v/release/UUDigitalHumanitieslab/datasette-matomo?include_prereleases&label=changelog)](https://github.com/UUDigitalHumanitieslab/datasette-matomo/releases)
[![Tests](https://github.com/UUDigitalHumanitieslab/datasette-matomo/workflows/Test/badge.svg)](https://github.com/UUDigitalHumanitieslab/datasette-matomo/actions?query=workflow%3ATest)
[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/UUDigitalHumanitieslab/datasette-matomo/blob/main/LICENSE)

Add Matomo Web Analytics tracking code to Datasette.

## Installation

Install this plugin in the same environment as Datasette.

    datasette install datasette-matomo

## Usage

Make your configuration available to the Datasette process as environment variables:

    MATOMO_SERVER_URL=https://example.com/
    MATOMO_SITE_ID=1

The server URL must include the final slash.

## Development

To set up this plugin locally, first checkout the code. Then create a new virtual environment:

    cd datasette-matomo
    python3 -m venv venv
    source venv/bin/activate

Now install the dependencies and test dependencies:

    pip install -e '.[test]'

To run the tests:

    pytest
