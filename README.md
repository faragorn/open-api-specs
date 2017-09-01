# OpenAPI Specifications

This is what my collection of [OpenAPI specs(formerly Swagger)](https://swagger.io/) for various Public APIs.
All of the API definitions will be contributed to a larger library: [https://github.com/APIs-guru/openapi-directory](https://github.com/APIs-guru/openapi-directory)

Feel free to contribute your API specifications, please see the [contributing guide](#contributing-guide)

## Index

| API | Description | Official Page |
| --------- | --------- | --------- |
| [Giphy API](specs/giphy_api) | World's largest gif collection | https://developers.giphy.com/docs/ |

## Contribing Guide

### Formatting

#### Folder name for the Specification

All specifications should be added under respective folder in `specs` directory. The name of the folder should match the name of the API, and should be always postfixed with `_api`. Example: folder name for Giphy API: `specs/giphy_api`. Note that the name of the folder is snake-cased.

#### API Versioning

All APIs often change and new versions emerge. To support this create a version folder in the respective API folder. It should be always followed by minor patch number even if it is `0`. If the API is not versioned, lets assume its' version is `1.0`. Example: Giphy API version is `1`, so the folder name should be: `specs/giphy_api/1.0`

#### Specification file
Specifications file should only be added under corresponding version number folder, described above. For single file specification filename should always be `index`. For multiple files, there should always be file named `index`. You specification can be represented in JSON or YAML formats. Example: `specs/giphy/1.0/index.yml`

#### Misc
Please make sure your passes Swagger parser validations and don't forget to add a line to a README.md file.
Please do not create a duplicate entry If the API is already described with OpenAPI, contribute to the existing specification instead.

### Pull Request
- Fork the repository and clone it locally. Connect your local repository to the original upstream repository by adding it as a remote. Pull in changes from upstream often so that you stay up to date and so when you submit your pull request, merge conflicts will be less likely.
- Create a branch for your edits.
- Contribute in the style of the project as outlined above. This makes it easier for the collaborators to merge and for others to understand and maintain in the future.
- When you are ready create a [Pull Request](compare)


