pipeline {
  agent any
  stages {
    stage('DB.Backup') {
      steps {
        cleanWs(cleanWhenAborted: true, cleanWhenFailure: true, cleanWhenNotBuilt: true, cleanWhenSuccess: true, cleanWhenUnstable: true, cleanupMatrixParent: true)
        bat '.\\DatabaseOp\\backup_2017db.bat 127.0.0.1 MSCSDB .\\DatabaseOp\\backup_2017db.bat 127.0.0.1 AMSDB'
      }
    }
  }
}