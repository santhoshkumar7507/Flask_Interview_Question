# Flask Forms

31. What is Flask-WTF?

Extension for handling forms securely.

Uses WTForms.

32. Why CSRF protection?

Prevents cross-site request forgery attacks.

33. What is form validation?

Ensuring user input is correct before processing.

34. Example validator
DataRequired()
Email()

35. How to display errors?
{{ form.username.errors }}

# Sessions and Cookies

36. What is session in Flask?

Session stores user data between requests.

37. Example
session['user'] = "admin"

38. Where session data is stored?

By default in secure cookies.

39. What is SECRET_KEY?

Used to encrypt session data.

40. Difference between cookies and sessions?

Cookies → client-side
Session → server-managed