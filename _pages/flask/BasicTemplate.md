---
layout: post
meta: 'Flask Basic Template'
categories: "flask"
source: "Codemy.com Youtube"
---

# Basic Template

```
# Create a really simple web site with Flask

from flask import Flask, render_template

# Create a Flask Instance
app = Flask(__name__)

# Create a route decorator. A route is equivalent to index.html, about.html, etc.
# So in this case it's the root of the website.
@app.route("/")

def index():
    return "<h1>Hello World!</h1>"

```