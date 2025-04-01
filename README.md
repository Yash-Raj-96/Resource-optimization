# API for Resource Optimization

## Project Overview

The **Resource Optimizer API** is a system designed to optimize the usage of system resources such as CPU, memory, and temporary files for improved performance and efficiency. This API allows users to interact with the system's resource management features through a set of RESTful API endpoints, offering solutions for real-time optimization of resources.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Software Requirements and Installation Procedures](#software-requirements-and-installation-procedures)
3. [Source Code Link (GitHub)](#source-code-link-github)
4. [Description About Each Module](#description-about-each-module)
5. [Implementation Details and Tools Used](#implementation-details-and-tools-used)
6. [Working Procedure](#working-procedure)
7. [Conclusion](#conclusion)

---

## Introduction

In the context of server and application management, **Resource Optimization** ensures that computing resources like CPU, memory, storage, and network bandwidth are allocated efficiently to maximize performance and minimize costs. This API helps in dynamic management of resources, offering techniques such as load balancing, autoscaling, and monitoring to prevent performance degradation, downtime, and excessive costs.

---

## Software Requirements and Installation Procedures

Below is a list of software required to set up and run the project:

| **Software**         | **Version**         | **Installation Link**                                                | **Purpose**                                                    |
| -------------------- | ------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------- |
| Java Development Kit | 11 or higher        | [JDK 11](https://www.oracle.com/java/technologies/downloads/#java11) | Development environment for Java applications.                 |
| Spring Boot          | 2.6.7 or compatible | [Spring Initializr](https://start.spring.io/)                        | Framework for building RESTful APIs and microservices.         |
| Eclipse IDE          | 2023-03 or higher   | [Eclipse IDE](https://www.eclipse.org/downloads/)                    | Integrated development environment (IDE) for Java development. |
| Maven                | 3.8.6 or higher     | [Maven](https://maven.apache.org/download.cgi)                       | Build tool for managing dependencies and project lifecycle.    |
| Postman              | 10.1 or higher      | [Postman](https://www.postman.com/downloads/)                        | Tool for testing and interacting with APIs.                    |

---

## Source Code Link (GitHub)

You can access the source code for this project on GitHub:

[GitHub Repository](https://github.com/Yash-Raj-96/Resource-optimization.git)

---

## Description About Each Module

### 1. TargetHealthController Class (API Endpoint)

The **TargetHealthController** class handles system resource allocation, including CPU, memory, storage, and bandwidth. It dynamically adjusts resource allocation based on demand or predefined thresholds.

### 2. MetricsAnalyzerService Class

This service monitors and analyzes system metrics like CPU, memory, disk I/O, and network bandwidth. It detects anomalies, bottlenecks, or inefficiencies that could impact system performance.

### 3. HTML Frontend

The **HTML frontend** displays real-time system metrics and provides an interface to optimize resources. It interacts with backend services via APIs to fetch live data and trigger optimization actions.

### 4. `pom.xml` (Maven Project Object Model)

The `pom.xml` file manages project dependencies and build configurations, ensuring that the necessary libraries, like Spring Boot, are included.

---

## Implementation Details and Tools Used

### 1. Spring Boot Framework

- **Purpose**: Used for developing the backend of the application with minimal configuration.
- **Implementation**: Utilizes Spring Boot's Starter Web dependency to handle HTTP requests and expose RESTful API endpoints.

### 2. REST API (Spring MVC)

- **Purpose**: Implements the REST API that exposes endpoints for system metric retrieval and resource optimization.
- **Implementation**: `/api/cpu-usage` and other endpoints allow resource optimization tasks such as scaling CPU and memory usage.

### 3. Frontend for Metrics Usage (HTML/CSS)

- **Purpose**: A simple webpage to display system metrics.
- **Implementation**: HTML form displays metrics like CPU usage, memory, and disk usage, and provides options to trigger optimization actions.

### 4. Maven for Dependency Management

- **Purpose**: Manages the project's dependencies and builds the application efficiently.
- **Implementation**: Dependencies such as `spring-boot-starter-web` and `tess4j` are included in the `pom.xml` file.

---

## Working Procedure

The **Resource Optimizer API** works by collecting real-time system metrics, displaying them via a frontend interface, and providing actions to optimize resource usage.

### Backend Setup

- **Metrics Collection**: A service collects system metrics such as CPU, memory, and disk usage.
- **Optimization Service**: The API endpoints allow users to optimize resources (e.g., scale CPU or memory).
- **Temp File Cleanup**: A service that clears unnecessary temporary files and cache.

### Frontend

- The HTML page displays metrics and allows users to trigger resource optimization actions through buttons.
- **Backend Interaction**: The frontend sends requests to the backend API to fetch and optimize system metrics.

---

## Conclusion

The **Resource Optimizer API** efficiently manages and optimizes system resources, improving performance and reducing operational costs. Through real-time monitoring, resource allocation, and cleanup actions, this API ensures optimal system performance. By combining backend services with a user-friendly frontend interface, it provides users with an effective tool to manage system resources seamlessly.

This project serves as a foundational tool for managing system resources, and it can be extended to incorporate more features as system demands evolve.

---

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
