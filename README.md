# CBECC Res CF1R Reporting Schema

## Contributing

Thanks for your interest in contributing! There are many ways to contribute to this project.
Get started here [CONTRIBUTING](CONTRIBUTING.md)

The current process uses the `schema` folder as the original set of schema files.
The processed and usable schema are in the `deployed` folder.

## Deploy Schema

`deploy-schema.exe` is a command line application executable file that was
written in [Golang](https://golang.org/). This application deploys the schema (replaces embedded
square markup, formats, indents, removes whitespace, orders alphabetically)
to a `deployed` folder.  There is also a `deploy-schema` script that runs
on Linux and MacOS.

### Windows

```
$ deploy-schema.exe
Usage: deploy-schema.exe [options]
Options:
  -d, --destination string
        Path to deploy the schema:
  -s, --source string
        Path to schema:
  -v, --version string
        Enter new schema version:
```

#### Example run

```
cd CBECC-Res-CF1R-Reporting-Schema
deploy-schema.exe -d . -s schema -v 2019.1.000
```
