pipeline
{
    agent{
        node {label 'workstation'}
    }

    stages{

        stage('Unit tests'){
            steps{
             echo 'Unit tests'
            }
        }

        stage('Code Analysis'){
            steps{
             sonar-scanner -Dsonar.host.url=http://172.31.20.113:9000 -Dsonar.login=admin -Dsonar.password=admin123 -Dsonar.projectKey=frontend
            }
        }

        stage('Security Scans'){
            steps{
             echo 'Security Scans'
            }
        }

        stage('Publish a Artifact'){
            steps{
             echo 'Publish a Artifact'
            }
        }
    }
}