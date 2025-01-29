# 33902

## Current behavior

Renovate cannot find the `requirements.in` file.  Notice the extra `requirements/` in the path.

```log
DEBUG: pip-compile: No content for source file requirements/requirements/requirements.in (repository=local)
```

## Expected behavior

Renovate should find the requirements file.

## Running locally with Docker

Fill the value for `GITHUB_COM_TOKEN`!

```bash
docker run -it --rm -e LOG_LEVEL=debug -e GITHUB_COM_TOKEN="..." -e RENOVATE_CONFIG_FILE=renovate.json -v "$(pwd):/usr/src/app" renovate/renovate:39.137
```

## Link to the Renovate issue or Discussion

https://github.com/renovatebot/renovate/discussions/33902
