Orchestration for a Simple Spring Rest App
==========================================
This contains a simple configurtation file to drive the the build and deployment
of a [Simple Spring Rest App][1].

Installation
------------
You will need Docker and [fig][2] installed.

To Run
------
Use the following:

	MYSQL_ROOT_PASSWORD=test fig -p dockerfortheenterprise up

To Build Images from Source
---------------------------
You will want to replace one of the lines in the `fig.yml` file so that it
references the submodule directly (instead of fetching it from the Docker repo).

Replace:

	image: zanegrey/simple-spring-rest-app-builder

With:

	build: app-builder

[1]: https://github.com/docker-for-the-enterprise-demo/simple-spring-rest-app
[2]: http://www.fig.sh/
