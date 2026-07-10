pipeline { //pipleline
    agent {label 'python-worker1-ec2'}
    stages { //collection of jobs/stage
                stage('Deploy the app in dev env'){
            steps{
                sh 'docker pull him111/gfgpython43cicd:latest'
                sh 'docker rm -f webapp'
                sh 'docker run -dit --name webapp -p 80:80 him111/gfgpython43cicd:latest'
            }
        }
    }
}
