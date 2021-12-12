# social-places
SocialPlaces project for the Sistemi Context-Aware (Context-Aware Systems) course of University of Bologna, A.Y. 2020/2021

In this project we present a **social-, location- and activity-aware** platform together with **anonymization of sensitive data** of the user.
Thanks to the combination of these three principles we have built an application, with private and public aspects, for places recommendation, personal
agenda and a social system.

## Prerequisites
To correctly make use of this project one needs the following software installed on their system:

- [Android Studio](https://developer.android.com/studio), for the mobile application ([/app folder](https://github.com/riccardopreite/sistemiCA-project))
- [Docker](https://www.docker.com/), for the backend ([/server folder](https://github.com/riccardopreite/sistemiCA-server))
- [Python](https://www.python.org/), for the dataset generation ([/dataset-generation folder](https://github.com/riccardopreite/geolife_training)) and the backend development
- [Node.js](https://nodejs.org/), for the backend development

## Building
First of all, if you download/clone this repository and you see the folders `app/`, `dataset-generation/`, `report/`, `server/` that are empty, please run the following commands:
```bash
git submodule init
git submodule update
```

To build the server, from within the `server/` folder, type:
```bash
docker-compose up --build -d
```
For killing the running server use the following instead: `docker-compose down`.

To build the application, open the `app/` folder with **Android Studio** and then build it from there.
Otherwise one could also, from within the `app/` folder, type:
```bash
./gradlew build
```