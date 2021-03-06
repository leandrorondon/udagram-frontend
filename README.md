# Udagram Frontend

This project is part of my Capstone Project for [Udacity's Cloud Developer Nanodegree](https://www.udacity.com/course/cloud-developer-nanodegree--nd9990).

Udagram is a simple cloud application developed along side the Udacity Cloud Engineering Nanodegree.
It allows users to register and log into a web client and post photos to the feed.

The project is split into two parts:
1. This Frontend
A basic Ionic client web application, bootstrapped from [Udacity Simple Frontend](https://github.com/udacity/cloud-developer/tree/master/course-02/exercises/udacity-c2-frontend).
2. [The Serverless API](https://github.com/leandrorondon/udagram-serverless-go), a serverless API running on AWS.

## Getting Setup

> _tip_: this frontend is designed to work with [The Serverless API](https://github.com/leandrorondon/udagram-serverless-go). It is recommended you stand up the backend first, test using Postman, and then the frontend should integrate.

### Installing Node and NPM
This project depends on Nodejs and Node Package Manager (NPM). Before continuing, you must download and install Node (NPM is included) from [https://nodejs.com/en/download](https://nodejs.org/en/download/).

### Installing Ionic Cli
The Ionic Command Line Interface is required to serve and build the frontend. Instructions for installing the CLI can be found in the [Ionic Framework Docs](https://ionicframework.com/docs/installation/cli).

### Installing project dependencies

This project uses NPM to manage software dependencies. NPM Relies on the package.json file located in the root of this repository. After cloning, open your terminal and run:
```bash
npm install
```
>_tip_: **npm i** is shorthand for **npm install**

### Configure The Backend Endpoint
Ionic uses environment files located in `./src/environments/environment.*.ts` to load configuration variables at runtime. By default `environments.ts` is used for development and `environments.prod.ts` is used for produciton. The `apiHost` variable should be set to your server url either locally or in the cloud.

***
### Running the Development Server
Ionic CLI provides an easy to use development server to run and autoreload the frontend. This allows you to make quick changes and see them in real time in your browser. To run the development server, open terminal and run:

```bash
ionic serve
```

### Building the Static Frontend Files
Ionic CLI can build the frontend into static HTML/CSS/JavaScript files. These files can be uploaded to a host to be consumed by users on the web. Build artifacts are located in `./www`. To build from source, open terminal and run:
```bash
ionic build
```
***

## @TODO
2. Tasks
    i. Setup
        a. Clone, set up protected branches (dev, staging, master)
        b. NPM, Ionic CLI
        c. run tests (npm test), identify broken function, fix the function
        d. write tests for form validation and re-run tests
