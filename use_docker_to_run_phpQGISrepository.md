### Use docker-compose and php-apache to run the script

If you don't have PHP or a working web server running, you can use docker-compose to run phpQGISrepository with php-apache.  If you have a running PHP web server, you don't need this. Here is how to run `php-apache` with `docker-compose` to get phpQGISrepository running:

|**In Linux** |**In Windows**|
|---------|----------|
|*How to start the docker image*|*How to start the docker image*|
| <ul><li>Make sure Docker is running</li></li><li>Do the same steps as in the [general install instructions](README.md)</li><li>Go to the folder where you extracted the script.</li><li>Run `sudo docker-compose up -d` in the Terminal</li> <br /><br />Now your repository is available on `http://hostname:8082`. If you don't know where that is, it will probably be http://localhost:8082.| <ul><li>Make sure Docker is running</li><li>Do the same steps as in the [general install instructions](README.md)</li><li>Make sure Docker is running</li><li>Go to the folder where you extracted the script.</li><li>Run `docker-compose up -d` in Windows command line</li> <br /><br />Now your repository is available on `http://hostname:8082`. If you don't know where that is, it will probably be http://localhost:8082.|
|*How to stop the docker image*|*How to stop the docker image*|
| <ul><li>Run `sudo docker-compose stop qgis-repo` in the Terminal</li></ul>| <ul><li>Run `docker-compose stop qgis-repo` in Windows command line</li></ul>|

The YML file used to use docker-compose to run phpQGISrepository was created by [Nils Nolde](https://gitlab.com/nilsnolde) (@nilsnolde).