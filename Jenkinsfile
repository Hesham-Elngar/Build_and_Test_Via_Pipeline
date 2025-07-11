pipeline{
    agent any
    tools {
        maven 'Maven_3.9.9'
    }
    stages{
        stage('build'){
            steps{
               // git branch: 'main', url: 'https://github.com/Hesham-Elngar/Build_and_Test_Via_Pipeline.git'
                bat 'mvn clean package -Dskiptests=true'
            }
        }
        stage('test'){
            steps{
                bat 'mvn test'
            }
        }
    }
}
