# Udagram - Full-Stack Microservices Web Application

## Overview
A full-stack microservices-based web application for image sharing. This project leverages AWS EKS, Kubernetes, Docker, Typescript, and React.

## Note
The application runs on AWS infrastructure more specifically AWS EKS. To setup your AWS environment for the project, kindly refer to the [Official AWS Documentations](https://docs.aws.amazon.com/eks/latest/userguide/getting-started.html). Also configure your Kubernetes manifests using the appropriate image files.

## Infrastructure
The corresponding deployment and service configuration files are located in the [deployments](./deploy) directory. Also configure your AWS secrets as needed.

## Microservices Architecture

The application utilized the microservices architecture by dividing the components into separate microservices. The folder structure aligns with the design intention.
The repository is organized into four main folders: [udagram-api-feed](./udagram-api-feed), [udagram-api-user](./udagram-api-user), [udagram-frontend](./udagram-api-user), and [udagram-reverseproxy](./udagram-reverseproxy), each containing the implementation for the respective microservice or component.

### Udagram API - Feed

#### Overview
Handles the feed functionality of the application.

#### Setup
1. Navigate to the `udagram-api-feed` folder.
2. Install dependencies using `npm install`.
3. Configure environment variables in a `.env` file.
4. Run the API locally with `npm run dev`.

#### Deployment
Deploy the feed API microservice on AWS EKS:
1. Set up an AWS EKS cluster.
2. Deploy the feed API microservice using the Kubernetes manifests.

### Udagram API - User

#### Overview
Manages user-related functionalities.

#### Setup
1. Navigate to the `udagram-api-user` folder.
2. Install dependencies using `npm install`.
3. Configure environment variables in a `.env` file.
4. Run the API locally with `npm run dev`.

#### Deployment
Deploy the user API microservice on AWS EKS:
1. Set up an AWS EKS cluster.
2. Deploy the user API microservice using the Kubernetes manifests.

### Udagram Frontend

#### Overview
The frontend component of the Udagram application.

#### Setup
1. Navigate to the `udagram-frontend` folder.
2. Install dependencies using `npm install`.
3. Configure environment variables in a `.env` file.
4. Run the frontend locally with `npm start`.

#### Deployment
Deploy the frontend on AWS EKS:
1. Set up an AWS EKS cluster.
2. Deploy the frontend application using the Kubernetes manifests.

### Udagram Reverse Proxy

#### Overview
The reverse proxy server for load balancing across microservices.

#### Setup
1. Navigate to the `udagram-reverseproxy` folder.
2. The corresponding Dockerfile and nginx configuration are located there.

#### Deployment
Deploy the reverse proxy on AWS EKS:
1. Set up an AWS EKS cluster.
2. Deploy the reverse proxy server using the Kubernetes manifests.

## Contributing
We welcome contributions! Feel free to fork the repository, make your changes, and submit a pull request.

## Acknowledgements
We would like to thank [Udacity](https://udacity.com) and [ALX Africa](https://www.alxafrica.com/) for running the program which this project is a part of.
