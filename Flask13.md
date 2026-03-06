21. Create database connection.
app.config["SQLALCHEMY_DATABASE_URI"] = "sqlite:///db.sqlite"

22. Create model.
class User(db.Model):
    id = db.Column(db.Integer, primary_key=True)
    name = db.Column(db.String(100))

23. Insert record.
user = User(name="John")
db.session.add(user)
db.session.commit()

24. Fetch all users.
users = User.query.all()

25. Fetch single user.
user = User.query.get(1)

26. Update record.
user.name = "Mike"
db.session.commit()

27. Delete record.
db.session.delete(user)
db.session.commit()

28. Filter query.
User.query.filter_by(name="John").first()

29. Pagination.
User.query.paginate(page=1, per_page=10)

30. Count records.
User.query.count()