# Expert Level

91. What is Flask extension?

Reusable package that adds features.

92. How to create a custom extension?

Using Python packages integrated with Flask hooks.

93. What is dependency injection?

Passing dependencies rather than creating them inside functions.

94. How does Flask handle concurrency?

Depends on WSGI server.

95. What is application factory pattern?

<!-- Creates Flask app dynamically. -->

96. Example
def create_app():
    app = Flask(__name__)
    return app
    
97. What is Flask signal?

Event system for notifications.

98. How to version APIs?

Example:

/api/v1/users
/api/v2/users

99. What are microservices?

Independent services communicating via APIs.

100. How would you design a production Flask app?

Key components:

Flask API

PostgreSQL

Redis cache

Gunicorn

Nginx

Docker

CI/CD pipeline