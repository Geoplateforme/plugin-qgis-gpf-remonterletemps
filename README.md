# GPF - Remonter Le Temps - QGIS Plugin

[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
[![flake8](https://img.shields.io/badge/linter-flake8-green)](https://flake8.pycqa.org/)

## Generated options

### Plugin

> Here is a list of the options you picked when creating the plugin with the cookiecutter template.

| Cookiecutter option | Picked value |
| :------------------ | :----------: |
| Plugin name | GPF - Remonter Le Temps |
| Plugin name slugified | gpf_remonter_le_temps |
| Plugin name class (used in code) | GpfRemonterLeTemps |
| Plugin category | Web |
| Plugin description short | Consluter et comparer l'imagerie historique proposée par le site Remonter Le Temps de l'IGN |
| Plugin description long | Intégration du service RLT dans QGIS. |
| Plugin tags | IGN,Géoplateforme,remonter le temps,RLT,historique,imagerie,comparer |
| Plugin icon | default_icon.png |
| Plugin with processing provider | False |
| Author name | Julien Moura |
| Author organization | Oslandia |
| Author email | <qgis@oslandia.com> |
| Minimum QGIS version | 3.40 |
| Maximum QGIS version | 3.99 |
| Support Qt6 | True |
| Git repository URL | <https://github.com/Geoplateforme/plugin-qgis-gpf-remonterletemps> |
| Git default branch | main |
| License | GPLv2+ |
| Python linter | Flake8 |
| CI/CD platform | GitHub |
| Publish to <https://plugins.qgis.org> using CI/CD | True |
| IDE | VSCode |

### Tooling

This project is configured with the following tools:

- [Black](https://black.readthedocs.io/en/stable/) to format the code without any existential question
- [iSort](https://pycqa.github.io/isort/) to sort the Python imports

Code rules are enforced with [pre-commit](https://pre-commit.com/) hooks.  
Static code analisis is based on: Flake8

See also: [contribution guidelines](CONTRIBUTING.md).

## CI/CD

Plugin is linted, tested, packaged and published with GitHub.

If you mean to deploy it to the [official QGIS plugins repository](https://plugins.qgis.org/), remember to set your OSGeo credentials (`OSGEO_USER_NAME` and `OSGEO_USER_PASSWORD`) as environment variables in your CI/CD tool.

### Documentation

The documentation is generated using Sphinx and is automatically generated through the CI and published on Pages.

- homepage: <https://github.com/Geoplateforme/plugin-qgis-gpf-remonterletemps>
- repository: <https://github.com/Geoplateforme/plugin-qgis-gpf-remonterletemps>
- tracker: <https://github.com/Geoplateforme/plugin-qgis-gpf-remonterletemps/issues/>

----

## Next steps post generation

### 1. Set up development environment

> Typical commands on Linux (Ubuntu).

1. If you didn't pick the `git init` option, initialize your local repository:

    ```sh
    git init
    ```

1. Follow the [embedded documentation to set up your development environment](./docs/development/environment.md) to create  virtual environment and install development dependencies.
1. Add all files to git index to prepare initial commit:

    ```sh
    git add -A
    ```

1. Run the git hooks to ensure that everything runs OK and to start developing on quality standards:

    ```sh
    pre-commit run -a
    ```

### 2. Build the documentation locally

1. Have a look to the [plugin's metadata.txt file](gpf_remonter_le_temps/metadata.txt): review it, complete it or fix it if needed (URLs, etc.)., especially the `homepage` URL which should be to your GitLab or GitHub Pages.
1. Change the plugin's icon stored in `gpf_remonter_le_temps/resources/images`
1. Follow the [embedded documentation to build plugin documentation locally](./docs/development/documentation.md)

### 3. Prepare your remote repository

1. If you did not yet, create a remote repository on your Git hosting platform (GitHub, GitLab, etc.)
1. Create labels listed in [labeler.yml file](.github/labeler.yml) to make PR auto-labelling work.
1. Switch the source of GitHub Pages to `GitHub Actions` in your repository settings <https://github.com/Geoplateforme/plugin-qgis-gpf-remonterletempssettings/pages>
1. Add the remote repository to your local repository:

    ```sh
    git remote add origin <https://github.com/Geoplateforme/plugin-qgis-gpf-remonterletemps>
    ```

1. Commit changes:

    ```sh
    git commit -m "init(plugin): adding first files of GPF - Remonter Le Temps" -m "generated with QGIS Plugin Templater (https://oslandia.gitlab.io/qgis/template-qgis-plugin)"
    ```

1. Push the initial commit to the remote repository:

    ```sh
    git push -u origin main
    ```

1. Create a new release following the [packaging/release guide](./docs//development/packaging.md) with the tag `0.1.0-beta1` to trigger the CI/CD pipeline and publish the plugin on the [official QGIS plugins repository](https://plugins.qgis.org/) (if you picked up the option).

----

## License

Distributed under the terms of the [`GPLv2+` license](LICENSE).
