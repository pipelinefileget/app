pipeline {
    agent any
    environment {
    }
    stages {
        stage('pipelinetest') {
            steps {
                    sh """
                        oc login -u kubeadmin -p SwgA8-5SJZA-rLRUI-AZRzM
                        oc project dev04
                        oc new-app --name step1 --strategy=docker https://github.com/pipelinefileget/docker.git --allow-missing-images
                    """
            }
        }
    }
}

