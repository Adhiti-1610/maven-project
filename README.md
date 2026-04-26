# maven-project

trigger:
- main

pool:
  name: 'practice'

steps:
- script: mvn -version
  displayName: 'Check Maven'

- script: mvn clean package
  displayName: 'Build with Maven'
