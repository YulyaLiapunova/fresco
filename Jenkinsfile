pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Check Environment Variables') {
                    steps {
                        script {
                            echo "ANDROID_SDK_ROOT: ${env.ANDROID_SDK_ROOT}"
                            echo "JAVA_HOME: ${env.JAVA_HOME}"
                        }
                    }
                }
    }
}