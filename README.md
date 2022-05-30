# "Reacty" Python

## Excuse me, what?

So today I found [this cool post](https://dev.to/jennasys/creating-react-applications-with-python-2je1) on Dev.to.

I love React and I love Python, so why not try to join the two together and see how far we can push it? Brilliant!

This implementation utilizes the [transcrypt](https://www.transcrypt.org/home) library to act as a transpiler between Python and JavaScript, as well as the [Parcel](https://parceljs.org/) webpacker, which has built in support of transcrypt on build.

By setting these up, as well as our node dependcies, such as React and react-dom, we can essentially set up a Python entry (app.py) to build out React apps using Python instead of JSX.

## Making it Work

### Python env and dependencies

`$ python3.9 -m venv .venv` - create an environment

`$ source .venv/bin/activate` - activate your environment (windows may differ - please refer to venv docs if not using unix)

`$ python -m pip install -r requirements.txt` - install dependencies

### Node package and dependencies

`$ npm install` - grab your node dependencies. This should be all that's necessary

### Hit the "go" button

`npx parcel --no-cache index.html` - Start up the app using Parcel, with index.html as the entry. Using default settings, the site will be brought up to run at [localhost:1234](localhost:1234) on your machine.

## Attributions

[Creating React Applications with Python](https://dev.to/jennasys/creating-react-applications-with-python-2je1) - Really the main inspiration for this exploration. They did the big brain implementation and include a great walk through of setting this all up.
