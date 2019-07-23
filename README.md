# SonarScanner for application in GitlabCI

.gitlab-ci.yml
## Usage


```
stages:
  - ...
  - analyze
  - ...
  
analyze project:
  image: your-docker-registry.tld/path-to-image/sonar-runner
  stage: analyze
  script:
   - sonar-scanner
       -Dsonar.projectKey=YOUR_PROJECT_KEY
       -Dsonar.login=YOUR_PROJECT_LOGIN
```
