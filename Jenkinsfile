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
               echo '\033[34mHello\033[0m \033[33mcolorful\033[0m \033[35mworld!\033[0m'
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
