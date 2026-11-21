# dbt_home_credit

## project description

A Data Warehouse (DWH) project built with dbt (Data Build Tool) and PostgreSQL.

## Quick Start

1. Make sure the uv package maneger is installed:

```bash
uv --version
```

2. insatll the project dependencies (dbt and the PostgreSQL adapter):
   
```bash
uv sync
```

3. Clone reposetory and navigate to the project directory:

```bash
cd dbt_home_credit
```

## Configuration

Update the '~/.dbt/profiles.yml' configuration file with your database credentials.

## Main dbt Commands

- `dbt debug` - checks the connection to the data warehouse and validates the profile configuration.
- `dbt parse` - parses project files to check for configuration and syntax errors.
- `dbt compile` - compiles dbt models and generates SQL files.
- `dbt run` - materializes models as tables and views.
- `dbt test` - runs tests to validate data quality.
- `dbt seed` - loads data from CSV files into database tables.
- `dbt build` - the main command that combines run, test, and seed operations.
- `dbt docs generate` - generates project documentation.
- `dbt docs serve` - starts a local server to view the documentation.

Note: If the virtual environment is not activated, use `uv run dbt` instead of dbt to execute commands.