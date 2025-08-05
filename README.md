# Chat-Box
Real-time messaging web application
Using Spring Boot, WebSocket, and STOMP protocol.
It allows multiple users to chat with each other instantly without refreshing the page.
The app uses SockJS for fallback support, making it work even if WebSocket is not available in the browser.

project structure
src/main/java/com/prince/chatApp
│── ChatAppApplication.java        # Main Spring Boot entry point
│── config/WebSocketConfig.java    # WebSocket & STOMP configuration
│── controller/ChatController.java # Handles incoming & outgoing chat messages
│── model/ChatMessage.java         # Chat message data model
│
src/main/resources/static
│── index.html                     # Chat UI
│── app.js                         # Handles WebSocket connection & chat updates
│
pom.xml                            # Maven dependencies
