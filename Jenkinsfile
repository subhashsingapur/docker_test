pipeline {
    agent any

    stages {
        stage('Filecheck') {
            steps {
                script{
                    git_data = sh(script: 'git diff-tree --no-commit-id --name-only -r $GIT_COMMIT', returnStdout: true)
                    echo git_data
                }
            }
        }
    }
}
