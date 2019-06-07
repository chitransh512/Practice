// Declarative //
  pipeline {
agent any 
    environment { 
        CC = 'clang' 
    }
stages {
   stage('Example') {
environment {  
  DEBUG_FLAGS = '-g'
}
steps {
   sh 'printenv'
       }
    } 
 }
}
  // Script //
  node {
      /* .. snip .. */
      withEnv(["PATH+MAVEN=${tool 'M3'}/bin"]) {
          sh 'mvn -B verify'
      }
  }
