## Introduction

```sh
git clone <your_repo_url>
```

https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository 
    

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

