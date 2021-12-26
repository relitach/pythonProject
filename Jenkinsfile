properties([pipelineTriggers([pollSCM('* * * * *')])])
node{

    stage("clone"){
    checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/relitach/pythonProject.git']]])
    }
    stage("show files"){
    bat "dir"
    }
}