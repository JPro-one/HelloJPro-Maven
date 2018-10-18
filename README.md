# Note: The maven-plugin is still under development!



# HelloJPro-Maven

[![Build Status](https://travis-ci.org/jpro-one/HelloJPro-Maven.svg?branch=master)](https://travis-ci.org/JPro-one/HelloJPro-Maven)

This project, is a hello-world for [jpro, which enables javafx in the web.](https://www.jpro.one/)

[Here you can see this program running.](https://demos.jpro.one/helloworld.html)

More about JPRO: Website: [jpro.one](https://www.jpro.one/) - Twitter: [@jpro_one](https://twitter.com/jpro_one)

# How to start #

## Web Browser ##

### Start jpro in foreground (development mode) ###

```
mvn compile jpro:run
```


### Start jpro in background (server mode) ###

```
mvn compile jpro:restart
```


### Open jpro app in Web Browser ###
```
http://localhost:8080/index.html
```

### Show all jpro apps in Browser ####
```
http://localhost:8080/test/default
```

### Open jpro app in fullscreen ####
```
http://localhost:8080/test/fullscreen/[app-name]
```



