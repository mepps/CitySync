![Code for Baltimore](/docs/img/CfB.png)

## Documentation

## Setup
To run this locally the following software is required:
*  [Python](https://www.python.org/) (version minimum 3.6)
*  [Flask](https://palletsprojects.com/p/flask/)
*  [Flask-Marshmallow](https://flask-marshmallow.readthedocs.io)
*  [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com)
*  [Docker](https://docker.com) *optional*

### Local server
To run this application on your local machine you first need to install dependencies.  From the project root, run the following command:
```shell
pip install -r requirements.txt
```
(*note* in some environments you may need to run `pip3` instead of `pip` if you're running both Python 2.6 and 3.x.)

Once that completes you can run the application by running the following from the project root:
```shell
python server.py
```
(*note* in some environments you may need to run `python3` instead of `python` if you're running both Python 2.6 adn 3.x.)

#### Docker
Alternatively if you wish to run this in Docker instead of on your local you may do so using the included `Dockerfile`. To use the Docker simply run the following commands:
```shell
docker build -t citysync-dockerimg:latest .
docker run -d -p 5000:5000 citysync-dockerimg:latest
```
To stop the container run:
```shell
docker ps
```
Take note of the `CONTAINER ID` then run:
```shell
docker stop <container id>
```
You may then make changes to the code and re-run the initial `build` and `run` commands. 

## Using this product
Once setup and running (via Docker or locally) you can see the output by visiting http://localhost:5000

## Testing

## Sources and Links
