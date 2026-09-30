# HelloJPro-Maven

![CI Build](https://github.com/JPro-one/HelloJPro-Maven/actions/workflows/main.yml/badge.svg)

A hello-world for [JPro](https://www.jpro.one/), which runs JavaFX applications in the web browser.
The build is configured with Maven.

[See it running online.](https://demos.jpro.one/helloworld.html)

## Getting started

Run the app in development mode:

```shell
./mvnw jpro:run
```

Then open http://localhost:8080/index.html in your browser.

Start editing the page in `src/main/resources/one/jpro/hellojpro/fxml/HelloJPro.fxml`.
Its styles live in `src/main/resources/one/jpro/hellojpro/css/HelloJPro.css`,
and its logic in `src/main/java/one/jpro/hellojpro/HelloJProController.java`.

While developing, [CSSFX](https://github.com/McFoggy/cssfx) reloads the CSS in the running app
as soon as you save it (it is switched off in a `jpro:release` build).

To run it as a desktop app instead:

```shell
./mvnw javafx:run
```

To keep the server running in the background, use `./mvnw jpro:restart` and stop it with `./mvnw jpro:stop`.

## Deployment

Create a release zip:

```shell
./mvnw package jpro:release
```

It is written to `target/hellojpro-maven-jpro.zip`.
Copy it to your server, unzip it, and start the JPro server from the unzipped folder:

```shell
./bin/start.sh
```

Linux servers need some preparation first. See the Deployment chapter in the [JPro docs](https://www.jpro.one/docs/).

## More about JPro

 * Website: [jpro.one](https://www.jpro.one/)
 * Twitter: [@jpro_one](https://twitter.com/jpro_one)
 * Ticket System: [JPro-tickets](https://github.com/JPro-one/JPro-tickets)
