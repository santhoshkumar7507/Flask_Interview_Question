# Deployment Questions

61. Is Flask production ready?

Yes, but needs a production server.

62. Production server for Flask

Gunicorn

63. Web server for deployment

Nginx

64. Example deployment stack
Nginx → Gunicorn → Flask

65. What is Docker?

Containerization tool for deploying applications.

# Performance and Scaling

66. How to scale Flask?

Load balancing

Microservices

caching

67. Flask caching extension

Flask-Caching

68. What is Redis?

In-memory data store for caching.

69. What is rate limiting?

Prevent API abuse.

Library: Flask-Limiter

70. What is async support?

Flask supports async routes in newer versions.