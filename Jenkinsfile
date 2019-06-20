
node() {
    stage('Checkout') {
        checkout scm
        commit_hash = sh(script: 'git rev-parse --short HEAD', returnStdout: true).trim()
        echo "commit_hash: "+ commit_hash
    }
    stage("commit"){
        sh 'echo commit_hash'
    }
}
