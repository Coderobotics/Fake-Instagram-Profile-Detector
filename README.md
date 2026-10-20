# Fake Instagram Profile Detector

Fake Instagram Profile Detector is a Python and Flask machine learning web application that predicts whether an Instagram account is Real or Fake from its public profile metadata — profile picture presence, username/full-name digit ratios, bio length, follower/following ratio, privacy setting, and post count. Enter a username and the app fetches the profile and returns a verdict with a confidence score and a plain-English report explaining which signals drove it.

<img src="https://www.coderobotics.com/frontend/assets/icon/fake-instagram-profile-detector.jpg">

Manually eyeballing an Instagram account to guess if it's fake is unreliable and doesn't scale. Fake Instagram Profile Detector is a Flask web app backed by a trained RandomForest classifier that scores an account's likelihood of being fake purely from its public profile signals — no manual data entry, just type in a username.

What You Get
 
Detect by username only — enter a handle and the app fetches the account's public profile data automatically and analyzes it.
RandomForestClassifier trained on 11 behavioral/profile features (profile pic flag, username/name digit ratios, bio length, external URL presence, private flag, post/follower/following counts).
"Why this verdict?" report — alongside the Real/Fake call and confidence score, a checklist explains which specific signals (missing profile picture, digit-heavy username, thin bio, lopsided follower/following ratio, etc.) pushed the verdict.
Animated confidence ring and a single search-box UI — no sidebar, no extra menus.
Dark mode by default with a light-mode toggle (persisted per browser), glassmorphic gradient theme, Poppins + Inter typefaces.
AJAX-based results — no page reload.
Fully responsive — works on desktop and mobile.
Plus, included in the source:

Synthetic dataset generator modeled on the well-known Kaggle "Instagram Fake & Real Accounts" feature set.
Model training pipeline with evaluation, serialized via pickle.
Project report covering system design, features, algorithm, and evaluation.

Why This Toolkit?
 
Spotting fake or bot Instagram accounts by hand means checking follower ratios, bios, and post history one at a time — slow and inconsistent. This tool runs a trained classifier over the same signals instantly and explains its reasoning, so the verdict isn't a black box.

No manual feature entry — just a username
Confidence score, not just a binary label
Human-readable explanation of the verdict
Perfect For
 
Python/ML learners and final-year students
Social media trust & safety experimentation
Anyone needing a quick account-credibility check
Demonstrating a full ML pipeline: data generation ? training ? serving

Tech Stack
 
Python 3 + Flask
scikit-learn (RandomForestClassifier), pandas, numpy, joblib
RapidAPI Instagram Scraper (third-party lookup — keeps a real Instagram account from being flagged)
HTML/CSS/JS front end (Poppins + Inter, glassmorphic theme)

Prerequisites
 
Python 3.9+ installed and on your PATH
A free RapidAPI account and API key (for the username-lookup feature)

More details and download link:
https://www.coderobotics.com/product/fake-instagram-profile-detector
