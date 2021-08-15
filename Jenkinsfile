pipeline{

    agent any


    tools{
       nodejs 'NodeJS 4.8.6'
    }


    stages{
        stage('build'){
            steps{
                echo 'this is the build job'
                sh 'npm install'
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
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
 
