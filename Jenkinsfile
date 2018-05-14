pipeline {
    agent any
  
stages{
        stage('Init'){
            steps {
                echo "Testing..."
            }            }
        }

        stage ('Build'){
            parallel{
                stage ('Deploy to Staging'){
                    steps {
                        echo "Building..."
                    }
                }

                stage ("Deploy"){
                    steps {
                        echo "Code deployed..."
                    }
                }
            }
        }
    }
}