pipeline{
agent any
stages{
stage('clone'){
steps
git 'https://github.com/Bhargavi9949/first.git'
}
}
stage('Build){
steps{
echo 'Building the project...'
sh 'javac Welcome.java'
}
}
stage('Test'){
steps{
echo 'Running tests...'
sh 'java Welcome'
}
}
stage('Deploy'){
steps{
echo 'Deploying the project...'
}
}
}
post{
success{
echo 'Pipeline completed successfully'
}
failure{
echo 'Pipeline failed'
}
}
}
