# FlowAPI
Genomic Flow Application API

## Setup Environment

Setup the .venv 
```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

If necessary, setup bundler.
```bash
sudo apt-get update
sudo apt-get install ruby ruby-dev
sudo gem install bundler
bundle install --local path .gem
```

Set up hosting with Heroku (Automatic)
```bash
heroku login -i
bundle exec jekyll-auth setup --team_id 121500467
```

Set up hosting with Heroku (Manual)
```bash
heroku login -i
heroku create FlowAPI
heroku config:set GITHUB_TEAM_ID=121500467
git push heroku
heroku open
```