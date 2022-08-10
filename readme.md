# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

<!--**[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_-->

**Steps to install and Run Repo**

1. Install [Docker](https://docs.docker.com/get-docker/)
2. Verify docker is ready by running the following commands in your terminal: `docker -v` and `docker-compose -v`
3. Clone [Anythink Market repo](https://github.com/ObelusFamily/Anythink-Market-lorr7) if not cloned already in your local machine
4. Run `docker-compose up` from the project root directory to load Anythink's backend and frontend.
5. If Docker is working correctly, the backend should be running and able to connect to your local database. Test this by pointing your browser to `http://localhost:3000/api/ping`
6. check the frontend and make sure it’s connected to the backend. If you’ll be able to create a new user on `http://localhost:3001/register` then it's connected to backend.

> Just make sure that you run all scripts in the next quests on one of the containers created by docker-compose up.  Also, you can use docker exec to run commands on a running container.
