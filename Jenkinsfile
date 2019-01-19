def workspace
node
{
    stage('Checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/abhinaya1/test1.git']]])
        workspace = pwd()
    }
    stage('Static Code Analysis')
    {
        echo "Static Code Analysis"
    }
    stage('Build')
    {
        echo "Build the code"
    }
    stage('Unit testing')
        echo "unit testing"
    stage('Delivery')
    {
        echo "Deliver the code"
    }
}
