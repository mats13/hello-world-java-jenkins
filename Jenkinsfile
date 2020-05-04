pipeline {
 agent any
  stages {
   stage("clone") {
    steps {
						                
     sh "rm -rf *"
										                
     sh "git clone https://github.com/mats13/hello-world-java-jenkins"
    }
  }
  stage("build") {
   steps {
    sh "cd hello-world-java-jenkins/ && javac Main.java"
   }
  }
  stage("run") {
   steps {
    sh "cd hello-world-java-jenkins/ && java Main"
   }
  }
 }
}
