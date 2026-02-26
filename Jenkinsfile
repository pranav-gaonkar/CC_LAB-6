pipeline {
agent any

stages {

stage('Build Backend'){
steps{
script{
sh 'which docker || echo Docker not found'
sh 'docker version'
sh 'docker build -t backend-image ./backend'
}
}
}

stage('Run Nginx'){
steps{
sh 'docker run -d -p 8081:80 nginx'
}
}

}
}
