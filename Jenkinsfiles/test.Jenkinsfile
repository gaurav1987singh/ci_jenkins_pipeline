def test='mytest'
node {
stage('build'){
echo "Hello from build task"
gradle build -x test
    }
stage('unitTest'){
echo "Hello from unit task"
     }
stage('deploy'){
echo "Hello from deploy task"
  }
}
