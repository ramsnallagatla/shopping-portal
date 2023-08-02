pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('build'){
            steps{
                echo 'this is the first build job'
                sh 'npm install'
            }
        }
        stage('test'){
            steps{
                echo 'this is the second test job'
                sh 'npm test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the third package job'
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has been completed for shopping-portal...'
        }
        
    }
    
}
