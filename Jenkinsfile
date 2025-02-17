pipeline{
    agent any
    stages{
        stage("Restore Dependencies"){
            steps{
                bat 'dotnet restore'
            }
        }
        stage("Build project"){
            steps{
                bat 'dotnet build --configuration Release'
            }
        }
        stage("Run tests"){
            steps{
                bat 'dotnet test'
            }
        }
    }
}