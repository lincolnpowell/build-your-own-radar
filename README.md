# ThoughtWorks Radar
Please visit [thoughtworks/build-your-own-radar](https://github.com/thoughtworks/build-your-own-radar) for relevant documentation from the original project.

## i. Purpose
This document is aimed to familiarize and guide the reader about the ThoughtWorks Radar customization spike.

## ii. Conventions used in this document
None.

## iii. Requirements
1. Clone the [ThoughtWorks Radar](https://github.com/lincolnpowell/build-your-own-radar/tree/spike/customization) project
    ```shell script
    git clone https://github.com/lincolnpowell/build-your-own-radar.git
    ```
2. Install [Docker Desktop](https://www.docker.com/products/docker-desktop) 
3. Build Docker image
    ```shell script
    docker image build -t thoughtworks-radar --build-arg API_KEY=YOUR_GOOGLE_API_KEY --build-arg CLIENT_ID=YOUR_GOOGLE_CLIENT_ID -f ./Dockerfile .
    ```
   **NOTE:** You will need to add the [Google Sheets API library](https://console.developers.google.com/apis/library/sheets.googleapis.com) to your Google Developers console project.
4. Run Docker container
    ```shell script
    docker container run --rm -p 8080:80 -e SERVER_NAMES="localhost 127.0.0.1" thoughtworks-radar
    ```
5. Open browser to http://localhost:8080
6. Follow [How to Use](https://github.com/thoughtworks/build-your-own-radar#how-to-use) on how to generate a radar

## iv. Assumptions
This document serves to familiarize and guide the reader about the ThoughtWorks Radar customization spike and how to build the application locally.

This document assumes the reader has working knowledge of all required applications, concepts, tools and their commands, inputs and outputs.

## 1. Purpose
To provide a scaffold into the discovery of implementing a custom ThoughtWorks Radar visualization experience using ThoughtWorks' [thoughtworks/build-your-own-radar](https://github.com/thoughtworks/build-your-own-radar) project as a base.

## 2. Issues
Please visit [Issues](https://github.com/thoughtworks/build-your-own-radar/issues) for open and closed issues on the [thoughtworks/build-your-own-radar](https://github.com/thoughtworks/build-your-own-radar) project.