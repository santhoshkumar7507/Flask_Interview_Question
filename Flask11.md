1. Create a simple Flask app that returns "Hello World".
from flask import Flask

app = Flask(__name__)

@app.route("/")
def home():
    return "Hello World"

if __name__ == "__main__":
    app.run(debug=True)
2. Create a route that returns JSON data.
from flask import jsonify

@app.route("/api")
def api():
    return jsonify({"message": "Hello API"})
3. Create a dynamic route that accepts a username.
@app.route("/user/<name>")
def user(name):
    return f"Hello {name}"
4. Accept query parameters from URL.

Example: /search?q=python

from flask import request

@app.route("/search")
def search():
    query = request.args.get("q")
    return f"Search result for {query}"
5. Create a POST API.
@app.route("/login", methods=["POST"])
def login():
    return "Login successful"
6. Read JSON request data.
@app.route("/data", methods=["POST"])
def data():
    content = request.get_json()
    return content
7. Return custom HTTP status code.
return "Created", 201
8. Redirect to another route.
from flask import redirect

@app.route("/old")
def old():
    return redirect("/new")
9. Send HTML template.
from flask import render_template

@app.route("/")
def home():
    return render_template("index.html")
10. Handle 404 error.
@app.errorhandler(404)
def not_found(e):
    return "Page not found", 404
