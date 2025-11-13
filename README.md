# 🚀 Rails × Docker Starter Template

## Prerequisites
- Docker
- Git

## Usage
1. Clone the Repository.
```
$ git clone git@github.com:kchan-lab/docker-rails-template.git
$ cd your-project
```
2. Build Docker Containers & Install Gems.
```
$ docker compose build

// Full/Default Mode
$ docker compose run --rm web rails new . -T -d postgresql --force --skip-docker

// API Mode
$ docker compose run --rm web rails new . --api -T -d postgresql --force --skip-docker

$ docker compose run --rm web bundle install
```

3. Start the Application.
```
$ docker compose up -d
```