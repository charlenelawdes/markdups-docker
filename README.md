[![Build and Push Docker Image](https://github.com/bwbioinfo/<tool>-docker-cwl/actions/workflows/build-and-push.yml/badge.svg)](https://github.com/bwbioinfo/<tool>-docker-cwl/actions/workflows/build-and-push.yml)

# markdups-docker

This repository provides a container for running the mark-dups program from [hmftools](https://github.com/hartwigmedical/hmftools) program. The tool is packaged in a Docker container, allowing it to run on any system with Docker or Singularity installed.

## Prerequisites

To use this tool, you must have the following software installed on your system:
- [Docker](https://www.docker.com/) OR [Singularity](https://sylabs.io/singularity/) OR [Apptainer](https://apptainer.org/)

## Installation

To install and run the tool, follow these steps:

1. Clone this repository to your local machine.
2. Install Docker, if you haven't already done so.
3. Build the Docker image by running the following command from the root of the repository:

    ```
    docker build -f docker/Dockerfile -t markdups-docker .
    ```
    OR pull from the built container.
    ```
    docker pull ghcr.io/charlenelawdes/markdups-docker:latest
    ```

## Contributing

If you wish to contribute to this project, please follow the standard GitHub workflow:

1. Fork the repository
2. Create a new branch for your changes
3. Make your changes and commit them
4. Push your changes to your fork
5. Submit a pull request to this repository

## License

This project is licensed under the [MIT License](https://github.com/bwbioinfo/tool-docker-cwl/blob/main/LICENSE).

## Contact

If you have any questions or feedback, please contact the author via GitHub.
