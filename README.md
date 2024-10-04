# Helm Chart Repository for Resource Configuration for Kubernetes Environment

## 🔗 Authors
[![Github](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://www.github.com/viniciusmpacheco)
[![Linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/viniciusmpacheco)
## Repository Structure

The Helm Chart repository aims to contain dynamic configuration of resources applied to a Kubernetes environment on a cloud provider.
## Repository Structure

This repository contains the configurations for the charts that are part of it, as well as the packages that can be downloaded from the repository and managed locally by the Helm CLI.

The repository has a structure similar to the one described below:

```
charts/
├── index.yaml
└── helm-chart.0.0.0.tgz
helm-chart/
├── charts/
├── crds/
└── templates/
    └── NOTES.txt
├── Chart.yaml
├── values.yaml
├── values.schema.json
├── LICENSE
├── README.md
```

## Repository of Charts

The **charts** directory only houses compressed packages of the charts that are configured in the root of the directory, as well as the **index.yaml*** which is the file that allows indexing these packages.

**NOTE: Each chart has a respective package with the versioning according to the update of the corresponding chart settings.**

| Folder/File Name      | Description           |
|-----------------------|-----------------------|
| charts/               | Directory containing the indexing file for the repository's chart packages and their respective packages           |
| index.yaml            | File containing indexing information for each chart package           |

## Charts Resources

Every Helm Chart has a basic organization of files that allow the chart to function. Below are described the items that make up the chart.

**NOTE: Each chart's directory is located at the root of the repository.**

| Folder/File Name      | Description           |
|-----------------------|-----------------------|
| charts/               | A directory containing any charts upon which this chart depends |
| crds/                 | Custom Resource Definitions |
| templates/            | A directory of templates that, when combined with values, will generate valid Kubernetes manifest files |
| templates/NOTES.txt   | OPTIONAL: A plain text file containing short usage notes |
| .helmignore           | File containing files and folder that will be ignored by Helm durig your operation |
| Chart.yaml            | A YAML file containing information about the chart |
| values.yaml           | The default configuration values for this chart |
| values.schema.json    | OPTIONAL: A JSON Schema for imposing a structure on the values.yaml file |
| LICENSE               | OPTIONAL: A plain text file containing the license for the chart |
| README.md             | OPTIONAL: A human-readable README file |
