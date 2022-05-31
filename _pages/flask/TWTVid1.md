---
layout: "page"
meta: "Basic Template Flask Tech With Tim"
categories: "flask"
source: "Tech With Tim Youtube"
---


# TWT Vid1 Basic Template

```
# Video 1 in Tech With Tim Flask Playlist

from flask import Flask, redirect, url_for

app = Flask(__name__)

# Setup home page
@app.route("/")
def home():
    return "Hello! this is the main page <h1>HELLO</h1>"

# Page is whatever you type after the root i.e. localhost:5000/terry
@app.route("/<name>")
def user(name):
    return f"Hello {name}!"

# Redirect Page
@app.route("/admin")
def admin():
    # redirect takes the name of the function not the route i.e. home not "/"
    return redirect(url_for("home"))

if __name__ == "__main__":
    app.run()

```
