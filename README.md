## Introduction

## GitHub Actions

* Establish pipeline workflow for java maven configuration
* Strategy to run test for every pull request raised against master
* Run test in chrome browser in headless mode
* Publish Surefire reports

## Selenium Grid

* Implementation of Distributed Selenium Grid
* Enable cross browser/devices automation with different browser nodes
* Scalability
* Remote test executions

Open a command line/ Terminal in project folder
```standalone selenium grid in Mac
docker run -d -p 4444:4444 -p 5900:5900 -p 7900:7900 --shm-size 2g seleniarm/standalone-chromium:lates
```

```distributed selenium grid
docker compose -f docker-compose-v3.yml up -d
```
```scaling chrome service
docker compose -f docker-compose-v3.yml up --scale chrome=3 -d
```

```tear down containers
docker compose -f docker-compose-v3.yml down
```
