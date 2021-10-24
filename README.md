CalHacks 8.0 - 3rd Place Winner

Website-http://instapresent1.000webhostapp.com

# InstaPresent

This tool was built by Tanay

For more info, check out [our devpost](https://devpost.com/software/instapresent)

# How to run

This project requires two processes to run.

First, `git clone` our repository.

Then, create the virtualenv:

```bash
python3 -m pip install virtualenv
mkvirtualenv hack --python 3.6
source ~/hack/bin/activate
pip install -r ~/instapresent/reqs.txt
```

Then, open up tmux and run two sessions:

tmux pane 1:

```bash
cd ~/instapresent/data
source ~/hack/bin/activate
python3 server.py (requires restart on changes made to main_function.py)
```

tmux pane 2:

```bash
cd ~/instapresent/
source ~/hack/bin/activate
python3 manage.py runserver (does not require restart)
```
