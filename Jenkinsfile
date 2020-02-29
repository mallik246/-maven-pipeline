pipeline {

    agent any

    tools {

        maven 'Maven 3.6.3'

        jdk 'jdk8'

    }

    stages {

        stage ('pull from git') {

            steps {

                git 'https://github.com/mallik246/-maven-pipeline.git'

            }

        }

        stage ('Build') {

            steps {

                sh 'mvn clean compile package'

                sh 'java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App'

            }

        }

    }

}
