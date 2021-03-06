# TWEETBOT

### Objectivs
- [x] Follow Followers - followfollowers.py

    automatically follows anyone who follows you.
- [x] (F)ave star and retweet - favretweet.py

    automatically likes and retweets tweets that match certain criteria.

- [ ] Autoreply - nlp Knowledge needed
- [ ] tweet-cli - Ongoing


### Requirements
* Developer's API cerdential. Please visit [Twitter Developer Site](https://developer.twitter.com/)
* Python
* Docker Engine

## Directory Structure

```
├── Dockerfile
├── requirements.txt
├── config.py
├── favretweet.py
└── followfollowers.py
```

### USAGE:

#### Using Local/Remote machine:

```
$ pip install -r requirements.txt
$ export CONSUMER_KEY="<Cosumer Key>"
$ export CONSUMER_SECRET="<Consumer Secret>"
$ export ACCESS_TOKEN="<Access Token>"
$ export ACCESS_TOKEN_SECRET="<Access Token Secret>"
source .venv/bin/activate # if pyenv is in use
python followfollowers.py # or faveretweet.py
```

#### Using Docker-Container

##### Build the Docker Image
```
docker build -t fav-retweet-bot . 
```
##### Run the Docker Image
```
docker run -it -e CONSUMER_KEY="<Cosumer Key>" \
 -e CONSUMER_SECRET="<Consumer Secret>" \
 -e ACCESS_TOKEN="<Access Token>" \
 -e ACCESS_TOKEN_SECRET="<Access Token Secret>" \
 fav-retweet-bot
```

suggestions: Please open an issue and tag me @ashkankamyab