# tesla-prometheus-exporter

A Prometheus exporter for your Tesla.

Originally developed by [madchicken](https://github.com/madchicken/tesla-prometheus-exporter). I have now forked and continued development due to inactivity of the original repository.

## Usage

Firstly get a Tesla API token. The easiest way is to use this [utility on the Tesla-info.com website](https://tesla-info.com/tesla-token.php).

Then pass the token to the exporter.

    npm install
    npm run serve -- --token=qts-a0123456789

**Docker image & instructions coming soon.**

## Options

Some options can be set as environment variables instead of command line arguments.

- `--version` Show version number [boolean]
- `--token` TESLA API Token [required] (environment variable name: `TESLA_EXPORTER_TOKEN`)
- `--port` Used HTTP port for metrics export [default: 9898] (environment variable name: `TESLA_EXPORTER_PORT`)
- `--interval` Scraping interval in seconds [default: 120] (environment variable name: `TESLA_EXPORTER_INTERVAL`)
- `--vin` VIN of the car to be monitored. If not provided the fist one will be used. (environment variable name: `TESLA_EXPORTER_VIN`)
- `--debug` Debug mode (environment variable name: `TESLA_EXPORTER_DEBUG`)
- `--help` Show help
