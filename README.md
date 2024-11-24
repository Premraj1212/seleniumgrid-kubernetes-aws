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


## Java Installation

```
https://www.oracle.com/java/technologies/javase/jdk22-archive-downloads.html
```


## Use Intellij or Eclipse ? 
its best if you use Intellij for workshop to ensure everyone on same page

Directly import the project as a maven project

## Setup Project SDK
Intellij requires you to set/ choose project SDK , follow this link for the same, you should choose Java 22

https://intellij-support.jetbrains.com/hc/en-us/community/posts/360010215699-Set-up-a-project-SDK

## Download Maven

Download Maven https://maven.apache.org/download.cgi

Open a command line/ Terminal in project folder
```sh
mvn compile
```

If above command is successful then we are good to go

## Execution

```sh
mvn clean test
```

all the tests of mentioned suite in pom.xml will run

