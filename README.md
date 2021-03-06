# Mentimeter Voting Bot

[Mentimeter polls](https://www.menti.com/) is a website that allows polling and receiving votes from an audience. It is a great evening time pass to play with my friends but is often abused as a channel for bullying. Recently I had experiences with people intentionally putting questions just to demean others and bully those who chose a certain poll option. A very light example: not knowing what does POTUS or LOTUS stand for and then being made fun of. This repository provides a way to sabotage such malicious attempts at singling out people for their lack of general knowledge. Undoing a vote is not allowed by Menti, so atleast the users of this repo can immediately pollute the results if they perceive a threat to their opinion privacy.

This bot needs the id of the menti poll which is shared by the poll creator before they open the poll publicly accessible. The bot automatically scrambles the votes by casting numerous fake votes on vote options selected randomly hence rendering the poll creator unable to identify or single out a poll participant for their opinions.

## How to run

1. Install [chromedriver dependency](http://chromedriver.storage.googleapis.com/index.html) - download chromedriver, unzip, move to /usr/local/bin (Mac OS / Linux)

2. Install selenium: `pip install selenium`

3. Use `venv`:

```
vishwarajan-mbp:chrome_automation vishwarajanand$ virtualenv venv

# to open editor
(venv) vishwarajan-mbp:chrome_automation vishwarajanand$ code .

# to run
vishwarajan-mbp:chrome_automation vishwarajanand$ source venv/bin/activate
(venv) vishwarajan-mbp:chrome_automation vishwarajanand$ python web_bot.py
```

### Note

If mac stops `chromedriver` claiming "the developer cannot be verified", do the following steps:

1. `cd /usr/local/bin`
2. `xattr -d com.apple.quarantine chromedriver`

## Demo Video

[![Watch on YouTube](https://img.youtube.com/vi/8bqY13JOA_A/sddefault.jpg)](https://youtu.be/8bqY13JOA_A)

## Blog

Blog is published at: https://vishwarajanand.com/tech/released-mentimeter-voting-bot/
