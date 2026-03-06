# Database Integration

41. How to connect database in Flask?

Using extensions like:

Flask-SQLAlchemy

MySQL

PostgreSQL

42. What is ORM?

ORM maps Python objects to database tables.

43. What is SQLAlchemy?

A Python ORM library for database interactions.

44. Example model
class User(db.Model):
    id = db.Column(db.Integer, primary_key=True)
    name = db.Column(db.String(100))

45. What is migration?

Tracking database schema changes using Flask-Migrate.

# REST API with Flask

46. What is REST API?

REST is an architectural style for building web services.

47. HTTP methods used

GET

POST

PUT

DELETE

48. Flask extension for APIs

Flask-RESTful

49. Example API endpoint
@app.route('/api/users')
def users():
    return jsonify(users)

50. What is serialization?

Converting objects into JSON.
