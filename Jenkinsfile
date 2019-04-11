node {
stage('Unzip hybris') {
sh 'unzip -n /home/hybris/hybris-commerce-suite-6.2.0.0-COMM.zip'    
}

stage('Build section'){
  script {
  dir('hybris/bin/platform') {
  sh '. ./setantenv.sh'
  sh 'ant clean all'
    }
  }
}
}
