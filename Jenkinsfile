pipeline {
agent slave
tools {  
maven 'maven'
}

stages {

stage ('compile')
{
steps {

sh "mvn compile"

}
}

stage ('test')
{
steps {

sh "mvn test"
}
}

stage ('package')
{
steps {

sh "mvn package"
}
}

stage ('install')
{
steps {

sh "mvn install"
}
}
  stage("shell script"){
    steps{
      script{
        '''#!/bin/bash
        echo "hello world"
        '''

}
}

  }
}
}
