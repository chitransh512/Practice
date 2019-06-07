  // Declarative //
  pipeline {
agent any environment { 1
CC = 'clang' }
      stages {
          stage('Example') {
environment { 2 DEBUG_FLAGS = '-g'
}
steps {
                  sh 'printenv'
              }
} }
  }
  // Script //
  node {
      /* .. snip .. */
      withEnv(["PATH+MAVEN=${tool 'M3'}/bin"]) {
          sh 'mvn -B verify'
      }
  }
