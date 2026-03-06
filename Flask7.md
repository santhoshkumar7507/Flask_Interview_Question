# Security Questions

71. What is XSS?

Cross-site scripting attack.

72. What is CSRF?

Cross-site request forgery.

73. How does Flask prevent XSS?

Jinja auto-escapes HTML.

74. How to secure sessions?

Use:

HTTPS

strong SECRET_KEY

75. What is CORS?

Cross-Origin Resource Sharing.

Extension: Flask-CORS

# Testing

76. How to test Flask apps?

Using pytest.

77. Example test
def test_home(client):
    response = client.get('/')
    
78. What is test client?

Simulates HTTP requests.

79. What is mocking?

Replacing dependencies during testing.

80. Why automated testing?

Ensures application stability.