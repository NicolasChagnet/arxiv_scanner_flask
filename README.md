# arXiv daily RSS parser

This is a minimal Flask app which downloads the RSS feed from selected arXiv categories every day and presents them in a simple static website. It also allows for filtering by keywords, authors and between updated or new submissions.

This project is adapted from [zhuwenxing/daily_arxiv](https://github.com/zhuwenxing/daily_arxiv).

# How to use

The simplest way to spin this is to use [https://pythonanywhere.com](https://pythonanywhere.com). First make an account (the free tier is enough for this app) and follow these steps:
	
	- Download the contents of this repository. Create a file `password.txt` whose sole content is a password you wish to use to secure the parameters page.
	- Create a new web app, choosing the Flask option. This is so the routing is all set-up by the system.
	- Copy the contents of `flask_app.py` in the same file on the web app. Upload the other files and folders manually.
	- Set a daily task in order to execute `daily_download.py`, scheduled after the update of the rss feed (20:00 UTC-5).