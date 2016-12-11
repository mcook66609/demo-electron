node {
    checkout scm
    sh 'npm install'
    sh 'rpm run build-linux'
    dir('dist') {
      archiveArtifacts artifacts: '*.AppImage', fingerprint: true;
    }
}
