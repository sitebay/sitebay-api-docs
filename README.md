# Site Bay OpenAPI 3

This is the Site Bay API OpenAPI 3 Schema

## Requirements

The linter used for the OpenAPI spec is written in python3.
A virtualenv is recommended for local work.

```
virtualenv -p python3 venv
source venv/bin/activate
pip install -r requirements.txt
```

## Development

The spec can be linted using the `openapi3` module.

```
python -m openapi3 openapi.yaml
```

### Versioning

When making a new release you **must** tag the release with the correct semantic versioning-compliant version string so that all versions are populated appropriately.
There is a `./bin/deploy` helper which will help with this process.

```
./bin/deploy 0.1.0
```