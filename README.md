# GFE Service

### Swagger Server
This server was generated by the [swagger-codegen](https://github.com/swagger-api/swagger-codegen) project. By using the
[OpenAPI-Spec](https://github.com/swagger-api/swagger-core/wiki) from a remote server.

This example uses the [Connexion](https://github.com/zalando/connexion) library on top of Flask.

> This project has been tested on python 3.6.8

### Pre-requisites

- Your [imgt_db](https://hub.docker.com/r/nmdpbioinformatics/imgt_biosqldb/) should be running.
- Your [biosqldb](https://hub.docker.com/r/nmdpbioinformatics/gfe-db/) should be in running state.
- [py-gfe](https://github.com/nmdp-bioinformatics/py-gfe.git) should be updated with this 
[pull request](https://github.com/nmdp-bioinformatics/py-gfe/pull/31). Otherwise
you can run: `git clone -b feature/helper-act-service https://github.com/m-haziq/py-gfe.git` 
and install the update from local.

### Running the Server

In order to run the server, follow these steps in root directory of gfe-service:

- Create a virtual environment using python3 (preferable 3.6.8) and activate it:
```
virtualenv venv --python=python3
source venv/bin/activate
```
- Install requirements using:
```
pip3 install -r requirements.txt
```
- Run the server using:
```
python main.py
```

Your local server should be running at: [http://localhost:8080/ui/](http://localhost:8080/ui/)

### Further Details:

Your Swagger definition lives here: [http://localhost:8080/swagger.json](http://localhost:8080/swagger.json)

> Change debug=False in `main.py` for production.

~ Change Debug=False in production in `main.py`