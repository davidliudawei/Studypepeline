pipeline
{
  agent any
  parameters{
    string (name:'str',defaultValue:'default',description:'this is string param')
    booleanParam(name:'bool',defaultValue:'default',description:'this is bool param')
   text(name:'text',defaultValue:'text',description:'this is text param\\n next line')
    
  }
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
