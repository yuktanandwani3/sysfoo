pipeline{

   agent any

   tools{
       maven 'Maven 3.6.3' 
    }    

    stages{
        stage('build'){
            steps{
                echo 'compile maven app'
                sh 'mvn compile'
            }
        }
        stage('two'){
            steps{
                echo 'test maven app'
                sh 'mvn clean test'
            }
        }
        stage('three'){
            steps{
                echo 'package maven app'
                sh 'mvn package -DskipTests'
            }
        }
    }
      
}
