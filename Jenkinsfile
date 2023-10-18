pipeline{
    agent 'any'
    options{
    ansiColor('xterm') 
    }
    stages{
        stage('build'){
            steps{
                echo "hi"
            }
        }
        stage('test'){
            steps{
                echo '033 [31mHellooo033 [0m'
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
