# Brand Exports 
This application is the base application that loads all the sports data (Omniture, GolfNow, Kochava and Salesforce) and joins it with the classifier and writes to nbcuas-outbound/nbc sports/. Lastly, it writes a report file  to the directory. 

### Important Notes
There is one manual prep step for each time experian data comes in. 
It is <a href="http://datacluster.nbcuas.com/service/zeppelin-eng2/#/notebook/2D2Z5EM9P">here</a>.
    
### Testing and Compiling
```bash
> sbt clean coverage test 
> sbt coverageReport
> sbt coverageAggregate
``` 

### Deploying
```bash
cd $project-directory
sbt docker:publish
cd ./source/main/cd
./deploy.sh -e dev
``` 
### Scala Style
This project is setup with automatic Scala style checker, which examines your Scala code and indicates potential problems with it.


# tonyfraser.github.io
