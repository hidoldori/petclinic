pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install petclinic-app helm/petclinic  --set image.repository=registry.hub.docker.com/hidoldori/hidoldori --set image.tag=2'
              		//upgrade --install "헬름차트명" "헬름차트위치디렉토리"
            }           
        }
    }
}
