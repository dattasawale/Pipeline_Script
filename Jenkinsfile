pipeline  {
    agent any
    stages {
        stage('Git checkout') {
            steps {
                echo "Checking out done Git repo";
            }
        }
        
        stage('Buid') {
            steps {
                echo "Running Build.bat";
                bat 'Build.bat'
            }
        }
        
        stage('JUnit') {
            steps {
                echo "Running Unit.bat";
                bat 'Unit.bat'
            }
        }
        
        stage('Quality') {
            steps {
                echo "Running Quality.bat";
                bat 'Quality.bat'
            }
        }
        
        stage('Deploy') {
            steps {
                echo "Running Deploy.bat";
                bat 'Deploy.bat'
            }
        }
    }
}
