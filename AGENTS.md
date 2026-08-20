# Project: sfguide-data-engineering-with-coco

## Snowflake environment

- Database: `DEMO_DB`
- Schema: `TPCH_TRANSFORMED`
- Warehouse: `DEMO_WH`

## dbt

- Build all models: `dbt build --project-dir dbt/`
- Build a single model: `dbt build --select <model_name> --project-dir dbt/`
- Source data: `SNOWFLAKE_SAMPLE_DATA.TPCH_SF1` — all raw tables must be referenced through `_sources.yml`, never directly

## Conventions

- Model files use snake_case naming
- Feature branches follow the pattern: `feature/<description>`
- PRs are required before merging to main

## Tooling

- This project uses CoCo Desktop — do not use the `cortex` CLI command
