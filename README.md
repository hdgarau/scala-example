
# Using Scala and Codefresh to clone/package source code, and build a Docker image
![scala and Codefresh](images/scala-and-codefresh.png)

## The Example Scala Application

This project uses `Scala` to build an application which will eventually become a distributable Docker image.

In the root of this repository you'll find a file named `codefresh.yml`, this is our [build descriptor](https://codefresh.io/docs/docs/codefresh-yaml/what-is-the-codefresh-yaml/) and it describes the different steps that comprise our process.
Let's quickly review the contents of this file:

## Build in Codefresh

[Example pipeline](codefresh.yml)

See the [documentation](https://codefresh.io/docs/docs/learn-by-example/scala/scala-hello-world/) for more details.


## Build Locally

This is a simple example of how to create Docker image for a Scala
application.

To build the Docker image, run following command:

```
$ docker build -t codefresh-contrib/scala-hello-world-sample-app:1.0 .
```

To run the docker image, run following command:
```
$ docker run -it codefresh-contrib/scala-hello-world-sample-app:1.0
```
