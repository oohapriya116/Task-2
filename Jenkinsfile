pipeline { 
    agent any 
    stages{
        stage('Checkout') {
            steps{ 
                git branch: 'main', url: 'https://github.com/oohapriya116/Task-2.git' 
            } 
        } 
        stage('Install Dependencies') { 
            steps{ 
                bat 'pip install-r requirements.txt' 
            } 
        } 
        stage('Run Unit Tests'){ 
            steps{ 
                bat 'pytesttest_app.py-v' 
            } 
        } 
    } 
}