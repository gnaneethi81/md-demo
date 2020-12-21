pipeline{
    agent any
    stages{
      stage("Maven Build"){
         steps{
           echo "building maven project"
         }
      }
        stage("Deploy to Dev"){
            when{
              branch 'dev'
            }
         steps{
           echo "deploying to dev"
         }
      }
        stage("Deploy to qa"){
            when{
              branch 'qa'
            }
         steps{
           echo "deploying to qa"
         }
      }
        stage("Deploy to prod"){
            when{
              branch 'main'
            }
         steps{
           echo "deploying to production"
         }
      }
    }
}
