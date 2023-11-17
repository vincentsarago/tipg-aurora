
<p align="center">
  <p align="center">Aurora Backend for TiPG.</p>
</p>

---

**Documentation**:

**Source Code**: <a href="https://github.com/developmentseed/tipg-aurora" target="_blank">https://github.com/developmentseed/tipg-aurora</a>

---


## Install

```bash
git clone https://github.com/developmentseed/tipg-aurora.git
cd tipg-aurora

python -m pip install -e .
```

### Configuration

To be able to work, the application will need access to the database. `tipg-aurora` uses [Starlette](https://www.starlette.io/config/)'s configuration pattern, which makes use of environment variables or a `.env` file to pass variables to the application.

An example of a `.env` file can be found in [.env.example](https://github.com/developmentseed/tipg-aurora/blob/main/.env.example)

```
# you need to define the DATABASE_URL directly
DATABASE_URL=postgresql://username:password@0.0.0.0:5432/postgis
```

## Launch

```bash
$ pip install uvicorn

# Set your PostGIS database instance URL in the environment
$ export DATABASE_URL=postgresql://username:password@0.0.0.0:5432/postgis
$ uvicorn tipg-aurora.main:app
```

## Contribution & Development

See [CONTRIBUTING.md](https://github.com/developmentseed/tipg-aurora/blob/main/CONTRIBUTING.md)

## License

See [LICENSE](https://github.com/developmentseed/tipg-aurora/blob/main/LICENSE)

## Authors

Created by [Development Seed](<http://developmentseed.org>)

## Changes

See [CHANGES.md](https://github.com/developmentseed/tipg-aurora/blob/main/CHANGES.md).

