# Real-Time Chat Application 

A high-performance real-time chat application built with **Spring Boot** and **WebSocket**, utilizing the **STOMP** protocol for efficient message broadcasting.

##  Tech Stack
- **Backend:** Java 21, Spring Boot 3
- **Communication:** WebSocket, STOMP Protocol, SockJS
- **Frontend:** HTML5, CSS3, JavaScript (SockJS-client)
- **Build Tool:** Maven

##  Key Features
- **Real-Time Messaging:** Instant message delivery using WebSocket connection.
- **User Session Management:** Tracks user join/leave events via `SimpMessageHeaderAccessor`.
- **Public Broadcasting:** Uses an in-memory message broker to broadcast messages to all subscribers (`/topic/public`).
- **Fallback Support:** Integrated **SockJS** to support browsers without WebSocket capabilities.

##  How to Run
1. Clone the repository.
2. Run the application: `mvn spring-boot:run`.
3. Open `http://localhost:8080` in multiple browser tabs.
4. Enter a username and start chatting instantly!
