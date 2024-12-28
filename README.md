# IoT Network Simulation Platform

This platform enables users to design and simulate IoT networks with features similar to Cisco Packet Tracer. Users can add and connect IoT devices such as sensors and actuators, configure communication protocols like MQTT , and monitor real-time data traffic through WebSocket visualizations. The platform also supports detailed network analysis, providing tools to optimize IoT designs efficiently in a secure and interactive environment.

## Table of Contents
- [Software Architecture](#software-architecture)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Video Demonstration](#video-demonstration)
- [Contributing](#contributing)

## Software Architecture
The system architecture comprises a Spring Boot backend and a React frontend, communicating via REST APIs. WebSocket is used for real-time traffic visualization.

### Backend
The backend manages device configurations, network setup, and simulation processing. It includes:
1. **Controllers**: Handle API requests for device and network operations.
2. **Models**: Represent entities like IoT devices, sensors, actuators, and connections.
3. **Repositories**: Interface with the MySQL database for CRUD operations.
4. **Services**: Contain the core logic for simulation and communication protocol handling.

### Frontend
The React-based frontend provides:
- Intuitive UI for device placement and configuration.
- Real-time traffic visualization using WebSocket.

### Database
MySQL stores information on devices, users, and network setups. Schema auto-generation is handled by Spring Data JPA.

---

## Features
- **User Authentication**: Secure login and registration.
- **Device Addition**: Add devices like smart lights, sensors, and routers.
- **Network Configuration**: Set device IPs, SSIDs, and passwords.
- **Protocol Simulation**: Supports MQTT.
- **Traffic Visualization**: Real-time data packets flow displayed via WebSocket.
- **Start/Stop Simulation**: Buttons to control the simulation state.

---

## Technologies Used
### Backend:
- **Spring Boot**
- **MySQL**
- **WebSocket**

### Frontend:
- **React**
- **HTML/CSS**
- **JavaScript**

---

## Getting Started
### Prerequisites:
- **Git**: [Install Git](https://git-scm.com)
- **MySQL**: Ensure MySQL is running on port 3306.
- **Node.js**: Install using [Node.js LTS](https://nodejs.org).

### Steps:
1. Clone the repository:
    ```bash
    git clone <repository_url>
    cd <project_directory>
    ```
2. Setup the Backend:
    - Navigate to the backend directory:
      ```bash
      cd backend
      ```
    - Install dependencies:
      ```bash
      mvn clean install
      ```
    - Run the backend:
      ```bash
      mvn spring-boot:run
      ```
    - Verify the backend at [http://localhost:8000](http://localhost:8000).

3. Setup the Frontend:
    - Navigate to the frontend directory:
      ```bash
      cd frontend
      ```
    - Install dependencies:
      ```bash
      npm install
      ```
    - Run the frontend:
      ```bash
      npm start
      ```
    - Access the app at [http://localhost:3000](http://localhost:3000).

---

## Video Demonstration
(Optional) Record a video or screencast showcasing:
- Adding and connecting IoT devices.
- Configuring protocols like MQTT or HTTP.
- Real-time traffic visualization.

Ensure the video adheres to the following:
- MP4 format, max 150MB.
- Dimensions: 640x480 at 30 FPS.

Validate the video at [Elsevier's Video Validator](http://elsevier-apps.sciverse.com/GadgetVideoPodcastPlayerWeb/verification).

---

## Contributing
1. Fork the repository.
2. Create a new branch:
    ```bash
    git checkout -b feature-name
    ```
3. Commit your changes:
    ```bash
    git commit -m "Add feature-name"
    ```
4. Push to your branch:
    ```bash
    git push origin feature-name
    ```
5. Create a pull request for review.

---

Thank you for your contributions to IoT Network Simulation Platform!
