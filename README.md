# coding-project-template

# Back-End-Development-Songs

A Python Flask REST API project for managing song data using MongoDB. This project was developed as part of the IBM Back-End Development Capstone work.

## Environment Setup

This project was created from the provided coding project template.

### Python Version

The project uses Python **3.9.x**.

### Virtual Environment

Create and activate the Python virtual environment before installing the project dependencies.

The provided setup script can be executed with:

```bash
bin/setup.sh
```

The application requires a MongoDB service. The MongoDB connection is configured through the `MONGODB_SERVICE` environment variable.

Example:

```bash
export MONGODB_SERVICE=localhost:27017
```

## API

The application provides endpoints for working with songs, including:

* `GET /health` — check whether the service is running
* `GET /song` — retrieve songs
* `PUT /song/<id>` — update a song
* `DELETE /song/<id>` — delete a song

## Database

The Songs service uses **MongoDB** to store song information.

The application connects to the MongoDB service using the `MONGODB_SERVICE` environment variable.

## Testing

The REST API was tested using `curl`.

The tested functionality includes:

* Health check
* Retrieving songs
* Updating a song
* Deleting a song

Successful HTTP responses were verified for the required operations.

## Repository

This repository contains the Flask backend, MongoDB integration, and REST API implementation for the Songs service.
