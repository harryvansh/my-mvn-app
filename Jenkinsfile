pipeline {
    agent any 
    stages {
        stage('clone repo and clean') { 
            steps {
                 bat "mvn clean"
                // bat 'rmdir /s /q my-mvn-app' // Delete the directory
                // bat "C:\\Users\\harendrasinh.vansh\\AppData\\Local\\Programs\\Git\\cmd\\git.exe clone https://github.com/harryvansh/my-mvn-app.git"
                //bat "git clone https://github.com/harryvansh/my-mvn-app.git"
                //bat "C:\\apache-maven-3.9.3\\bin\\mvn clean -f my-mvn-app"
                //bat "mvn clean -f my-mvn-app"
            }
        }
        stage('Test') { 
            steps {
              bat "mvn test"
                // bat "mvn test -f my-mvn-app" 
            }
        }
        stage('Deploy') { 
            steps {
              bat "mvn package"
                // bat "mvn package -f my-mvn-app" 
            }
        }
    }
}
