pipeline{
    agent any
    stages{
        stage("Clone Repo"){
            steps{
                git branch: 'master', url: 'https://github.com/VivFifie/java-todo.git'
            }
        }
        stage("Build repo"){
            steps{
                sh "./gradlew clean build "
            }
        }
        stage("Test code"){
            steps{
                sh "./gradlew test"
            }
    }
}
