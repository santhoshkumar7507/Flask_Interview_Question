# Templates

21. What are templates?

Templates are HTML files with dynamic data rendered using Jinja2.

22. How to render a template?
render_template("index.html")

23. What are Jinja2 template features?

Template inheritance

Loops

Conditions

Filters

24. Example of Jinja loop
{% for item in items %}
{{ item }}
{% endfor %}

25. What is template inheritance?

Allows reuse of layout using base template.

# Flask Application Structure
26. Typical Flask project structure
app/
 ├ templates/
 ├ static/
 ├ app.py

27. What is static folder?

Stores:

CSS

JS

images

28. How to serve static files?
/static/style.css


29. What is Flask CLI?

Flask CLI provides commands like:

run

shell

routes

30. How to enable debug mode?
app.run(debug=True)