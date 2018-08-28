@Library('my-shared-libraries') _
def test='mytest'
node {
stage('build'){
echo "Hello from build task"
helloFromShared_Library(greetings)
echo "HOLA"
    }
stage('unitTest'){
echo "Hello from unit task"

     }
stage('deploy'){
echo "Hello from deploy task"
  }
}
