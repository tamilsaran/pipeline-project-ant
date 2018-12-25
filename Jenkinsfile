pipeline  {
     agent any

    stages {
     stage('build') {
       steps {
       sh 'ant -f build.xml -v'
       }
      }
	stage('test') {
	steps {
	sh 'ant -f test.xml -v'
	junit 'reports/result.xml'
	}
	}
    }
}
