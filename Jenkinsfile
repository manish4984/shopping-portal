pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('Build'){
            steps{
                echo 'this is the build job for lagairogo-shopping-portal'
                sh 'npm install'
            }
        }
        stage('Test'){
            steps{
                echo 'this is the test job for lagairogo-shopping-portal'
                sh 'npm test'
            }
        }
        stage('Package'){
            steps{
                echo 'this is the package job for lagairogo-shopping-portal'
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
