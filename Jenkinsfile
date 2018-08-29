@Library('my-shared-libraries') _
def test='mytest'
def properties
def serviceNameRepoUrlKey = "${SERVICE_NAME}"
node {
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
}
