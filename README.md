# ci-createmd

Drydock Create Markdown compliance tool.

This project follows the [Drydock Pattern](https://github.com/CivicActions/drydock#what-is-the-drydock-pattern).

## Getting Started

### Prerequisites

You will need to have Docker installed. See the [Install Docker docs](https://docs.docker.com/install/) for more information.

[Available on Docker Hub](https://hub.docker.com/r/drydockcloud/ci-secrender)

### CreateMD Operation

Copy the `docker-compose.example` file to your project and rename it `docker-compose.yml`.

Copy the `activate.example` file to your project and rename it `activate`.

#### To use **createmd**

```bash
# Activate Drydock
. activate

# Run createmd
createmd --in config.yaml --templates templates/
```

Running the above command will copy any files in the `/templates` directory, duplicating the template directory structure, into the current directory, replacing variables in the templates with the values from the `--in` file. You can also specify a directory in which to output the files using the `--out` option.

## Authors

* **Tom Wood** - *Initial work* - [Woodt](https://github.com/woodt)
* **Tom Camp** - [Tom-Camp](https://github.com/Tom-Camp)

## License

This project is licensed under the GNU General Public License - see the [LICENSE](LICENSE) file for details.
