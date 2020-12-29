# muttlib 🐶📚

[![pipeline status](https://gitlab.com/mutt_data/muttlib/badges/master/pipeline.svg)](https://gitlab.com/mutt_data/muttlib/-/commits/master)[![coverage report](https://gitlab.com/mutt_data/muttlib/badges/master/coverage.svg)](https://gitlab.com/mutt_data/muttlib/-/commits/master)

## Description

Library with helper code to start a data-related project.
By [Mutt Data](https://muttdata.ai/).

Current modules:

- `dbconn`: Somewhat homogeneus lib to access multiple DBs.
- `file_processing`: Helpers for concurrent file processing.
- `forecast`: Provides FBProphet a common interface to Sklearn and general
  utilities for forecasting problems, allowing wider and easier grid search for
  hyperparameters.
- `utils`: A single version of miscellaneous functions needed every now and then.
- `ipynb_const` and `ipynb_utils`: Utilities when doing exploratory work (helpful for jupyter notebooks).
- `gsheetsconn`: Module to make data interactions to/from Google Sheets <> Pandas.
- `gdrive`: Module that provides a UNIX-ish interface to GDrive.
- `gcd`: (Greatest Common Divisor, for lack of a better name - Ty @memeplex) Classes, abstract objects and other gimmicks.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [Credits](#contributing)
- [License](#license)

### Installing from PyPi
```bash
pip install muttlib
```

Check below for available extras.

### From repo

Base lib:

To install base lib:
```bash
pip install muttlib
```

Parquet and Feather support:
```bash
pip install muttlib[pyarrow]
```

IPython utils:
```bash
pip install muttlib[ipynb-utils]
```

Forecast:
```bash
pip install muttlib[forecast]
```

Misc DB support for dbconn:
```bash
pip install muttlib[oracle]
pip install muttlib[hive]
pip install muttlib[postgres]
pip install muttlib[mysql]
pip install muttlib[sqlserver]
pip install muttlib[moongo]
pip install muttlib[ibis]
```

Install custom branch from GitHub mirror:
```bash
pip install -e git+https://gitlab.com/mutt_data/muttlib.git@AWESOME_FEATURE_BRANCH#egg=muttlib
github.com/MuttData/muttlib
```

Install custom branch from Gitlab main repo:
```bash
pip install -e git+https://github.com/MuttData/muttlib.git@AWESOME_FEATURE_BRANCH#egg=muttlib
```

## Usage

See the [documentation](https://mutt_data.gitlab.io/muttlib/) to get started with `muttlib`.

## Contributing

We appreciate for considering to help out maintaining this project. If you'd like to contribute please read our [contributing guidelines](CONTRIBUTING.md).

## Credits

- Aldo Escobar
- Alejandro Rusi
- Cristián Antuña
- Eric Rishmuller
- Fabian Wolfmann
- Gabriel Miretti
- Javier Mermet
- Jose Castagnino
- Juan Pampliega
- Luis Alberto Hernandez
- Mateo de Monasterio
- Matías Battocchia
- Pablo Lorenzatto
- Pedro Ferrari
- Santiago Hernandez

## License
`muttlib` is licensed under the [Apache License 2.0](LICENCE).
