# AI Enterprise Workflow Capstone Project

This project involves time series analysis to predict revenue for the upcoming 30 days.

# Instructions for Use

All commands should be executed from this directory.

## Testing `app.py`

To run the application:

```bash
~$ python app.py
```

To enable debug mode while running the Flask app:

```bash
~$ python app.py -d
```

Access the web interface at http://0.0.0.0:8080/. You’ll find a basic website ready to be customized for your project.
    
## Testing and Training the Model

For model testing and training, refer to the code at the bottom of model.py:

```bash
~$ python model.py
```

## Building the Docker Container

To create the Docker container:

```bash
~$ docker build -t iris-ml .
```

Verify the created image:

```bash
~$ docker image ls
```

Remove unused images if necessary:

```bash
~$ docker image rm IMAGE_ID_OR_NAME
```

For periodic cleanup, you can run:

```bash
~$ docker system prune
```

## Running Unit Tests

Before executing unit tests, ensure app.py is running.

To test only the API functionality:

```bash
~$ python unittests/ApiTests.py
```

To test only the model functionality:

```bash
~$ python unittests/ModelTests.py
```

To run all available tests:

```bash
~$ python run-tests.py
```

## Testing the Docker Container

Run the Docker container to confirm functionality:

```bash
~$ docker run -p 4000:8080 iris-ml
```

Visit http://0.0.0.0:4000/ to see a basic website that you can adapt for your project needs.




