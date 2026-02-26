pipeline {
agent any
stages {
stage('Build Backend'){
steps{
sh 'docker build -t backend-image ./backend'
}
}
stage('Run Nginx'){
steps{
sh 'docker run -d -p 80:80 nginx'
}
}
}
}
