# Development mode

The following steps will guide you so that you can have a development environment on your machine without having to install Ghost:

1. Install [Docker](https://docs.docker.com/install/) and [docker-compose](https://docs.docker.com/compose/install/).

2. Install [Nodejs](https://nodejs.org/en/download/) and [npm](https://www.npmjs.com/get-npm).

3. Clone or download this repository.

5. Run `yarn`.

<!-- 6. Run `npm run get-database` to get the Ghost database dump. -->

7. Start Docker.

8. Run `yarn docker-watch`.

Now you have an instant development setup and when you make changes you will see them right into the browser (hot-reloading).

You can see your blog here: `http://localhost:2368` and you can access to the admin here: `http://localhost:2368/ghost`.


If you add new files you will need to run `docker-compose restart` manually, this is because of this (from Ghost docs):

> If you add any new files to your theme during development, you'll need to restart Ghost to see the changes take effect.

<!-- ## Production mode

When you're ready you can build the theme for production just by running `npm run production` (within the `src` directory).

This command will generate the file `liebling.zip` in the root of the theme directory. Now you can upload this file to your own Ghost instance 😎. -->