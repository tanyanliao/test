pipeline {
 agent any
tools{
    gradle "gradle"
 }
stages {
    stage('init') {
           steps {
            script{
              def dockerPath = tool 'docker' //全局配置里的docker
              env.PATH = "${dockerPath}/bin:${env.PATH}" //添加了系统环境变量上
            }
           }
    }

    stage('Build') {
        steps {
            script{
              sh "docker --version"
            }
        }
    }
  }
}
