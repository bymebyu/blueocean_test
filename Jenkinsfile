pipeline {
  agent any
  stages {
    stage('UPDATE_MERGE') {
      steps {
        build '00_ALPHA_TO_AE_MERGE_SOURCE'
      }
    }

    stage('BUILD_BIN') {
      steps {
        build '01_AE_Build'
      }
    }

    stage('UNIT_TEST') {
      steps {
        build '02_AE_Basic_UnitTest'
      }
    }

  }
}