pipeline{
agent any
parameters{
string(
name: 'BRANCH_NAME',
defaultValue: 'main',
description: 'Git branch to build'
)
}
stages{
stage('Build'){
steps{
sh 'mvn clean package'
}
}
stage('Test'){
steps{
sh 'mvn test'
}
}
}
}
