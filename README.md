
# Rails API

Rails API is responsible for receiving user questions, validating input, and forwarding the request to the Python AI service. It acts as a secure gateway between the user and the AI layer.

**Endpoint:**

POST /api/v1/questions


- Receives JSON question and store context.
- Sends the request to Python AI service.
- Returns formatted response to the user.

Pseudo-code or mock implementation is acceptable for this assignment.
