pipeline{
  agent none
  stages{
    stage("build stage"){
      steps{
        echo "this is build stage"
      }
    }
    stage("test stage"){
      parallel{
       stage("test 1"){
         steps{
          echo "this is test1 stage"
        }
       }
         stage("test 2"){
         steps{
          echo "this is test2 stage"
        }
       }
      }
    }
    stage("deploy stage"){
      steps{
        echo "this is deploy stage"
      }
    }
  }
}
