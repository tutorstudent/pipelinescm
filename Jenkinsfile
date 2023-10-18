pipeline{
    agent 'any'
    stages{
        stage('build'){
            steps{
                echo "hi"
            }
        }
        stage('test'){
            steps{
                echo "world"
            }
        }
         stage ('run other builds'){
            steps{
                build 'edh - ci'
                build 'edh-develop'
            }
         }   
    }
}
