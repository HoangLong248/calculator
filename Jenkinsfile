pipeline {
    agent any
    stages {
        stage ("Checkout") {
            steps {
                git url: "https://github.com/HoangLong698/calculator.git"
            }
        }
        
        stage ("Compile") {
            steps {
                sh "./mvnw compile"
            }
        }
        
        stage ("Unit test") {
            steps {
                sh "./mvnw test"
            }
        }
    }
}
