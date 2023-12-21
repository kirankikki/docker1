pipeline {
  agent any
  stages {
    stage('') {
      steps {
        sh '''gcloud auth configure-docker us-west1-docker.pkg.dev 
gcloud auth print-access-token|sudo docker login -u oauth2accesstoken --password-stdin https://us-west1-docker.pkg.dev
sudo docker build -t us-west1-docker.pkg.dev/seventh-magnet-407805/garkiran1/jenapp1:mynginx .
sudo docker push us-west1-docker.pkg.dev/seventh-magnet-407805/garkiran1/jenapp1:mynginx'''
      }
    }

  }
}