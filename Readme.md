# Quick Start

```bash
APP=deployhub

heroku create $APP -s cedar
heroku config:add GIT_REMOTE=https://nzoschke:PASSWORD@github.com/nzoschke/deployhub.git
git push heroku master

git remote add self https://$APP.herokuapp.com/$APP.git
git push self master
```