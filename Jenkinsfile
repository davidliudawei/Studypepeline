pipeline
{
  agent any
  
  stages{
  
  stage("打包"){
    steps{
   bat label:'',script: 'echo build'
    }
  }
    stage("fa bu"){
      steps{
        bat label:'', script:'echo devolpy'
      }
    }
  }
   post{
    always{
      bat label:'',script :'echo always'
    }
    
    success{
      bat label:'',script:'echo success'
      
  }
    
    failure{
      bat label:'',script:'echo failure'
    }
    
    aborted{
      bat label:'',script:'echo aborted'
    }
   }
}
