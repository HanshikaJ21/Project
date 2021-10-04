pipeline {
    agent any 
    stages {
        stage('Clone Repository & clean') { 
            steps {
              sh "git clone https://github.com/JasujaHanshika/The-sparks-Foundation-project.git"
              sh "mvn clean -f The-sparks-Foundation-project"
                // 
            }
        }
        stage('Test') { 
            steps {
              sh "mvn test -f The-sparks-Foundation-project"
                // 
            }
        }
        stage('Deploy') { 
            steps {
              sh "mvn package -f The-sparks-Foundation-project"
                // 
            }
        }
    }
}
