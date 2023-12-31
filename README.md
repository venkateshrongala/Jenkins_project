# Jenkins_project
  Containerized Web-based Application using (CI/CD) pipelines in Jenkins
# Following are the specifications of the lifecycle:
  1. Install the necessary software on the machines using a configuration management tool
  2. Git workflow has to be implemented
  3. CodeBuild should automatically be triggered once a commit is made to master branch or develop branch.
     a. If a commit is made to master branch, test and push to prod
     b. If a commit is made to develop branch, just test the product, do not push to prod
  4. The code should be containerized with the help of a Dockerfile.
  5. The Dockerfile should be built every time there is a push to GitHub.
     Use the following pre-built container for your application: hshar/webapp
     The code should reside in '/var/www/html'
  6. The above tasks should be defined in a Jenkins Pipeline with the followingjobs:
      a. Job1 : build
      b. Job2 : test
      c. Job3 : prod
