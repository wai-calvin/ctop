pipeline {
  agent any
  
  environment {
    PATH+EXTRA = '/working_dir/go/bin'
  }

  stages {
    stage('Compile') {
      steps {
        sh 'go build'
      }
    }

    stage('Test') {
      steps {
        sh 'go test ./...'
      }
    }

    stage ('Release') {
      when {
        // A simple condition that just checks if the Pipeline is running against a tag in SCM, rather than a branch or a specific commit reference
        buildingTag()
        
      }

      // environment {
      //   GITHUB_TOKEN = credentials('github-token')
      // }

      steps {
        sh 'curl -sL https://git.io/goreleaser | bash'
      }
    }
  }
}