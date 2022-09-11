pipeline{
  agent any
    stages{
      stage("Maven Build"){
        when{
          branch "develop"
        }
      steps{
        echo "maven clean package....."
      }
    }
    stage("Solar Analysis"){
        when{
          branch "develop"
        }
      steps{
        echo "Sonar analysis....."
      }
    }
  stage("Dev deploy"){
        when{
          branch "develop"
        }
        steps{
          echo "deploying to dev......"
        }
  }
  stage("Prod deploy"){
        when{
          branch "main"
        }
        steps{
          echo "deploying to prod......"
    }
}
    }
}
