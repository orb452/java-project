pipeline {
agent any
stages {
stage('Build') {
steps {
sh 'ant -f build.xml -v'
echo 'Building..'
}
}
}
post {
	always {
        
          archiveArtifacts artifacts: 'dist/*.jar'
        }
      }
    }

