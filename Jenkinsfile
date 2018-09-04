@Library('my-shared-libraries') _
def test='mytest'
def properties
def serviceNameRepoUrlKey = "${SERVICE_NAME}RepoUrl"
node {
properties=loadProperties()

echo "The serviceNameRepoUrlKey: ${serviceNameRepoUrlKey}"
echo "Properties value: ${properties}"

stage('checkout'){
checkoutRepo(BRANCH, properties[serviceNameRepoUrlKey])
}
stage('build'){
echo "Hello from build task"
doBuild(WORKSPACE)
    }
stage('unitTest'){
echo "Hello from unit task"

     }
stage('deploy'){
echo "Hello from deploy task"
  }

 stage('Build_Number'){
evenOrOdd(currentBuild.getNumber())
 }
}
