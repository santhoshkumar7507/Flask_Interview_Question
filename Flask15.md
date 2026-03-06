41. Create REST API endpoint.
@app.route("/users", methods=["GET"])

42. Return JSON list.
return jsonify(users)

43. Create POST API.
@app.route("/users", methods=["POST"])

44. Update user API.
@app.route("/users/<int:id>", methods=["PUT"])

45. Delete API.
@app.route("/users/<int:id>", methods=["DELETE"])

46. API versioning.
/api/v1/users

47. API error response.
return jsonify({"error": "Invalid input"}), 400

48. API pagination.
limit = request.args.get("limit")

49. Rate limiting using Flask-Limiter
@limiter.limit("10/minute")

50. Enable CORS using Flask-CORS
CORS(app)