pipeline
{
  agent any
  parameters{
    string (name:'str',defaultValue:'default',description:'this is string param')
    booleanParam(name:'bool',defaultValue:'default',description:'this is bool param')
   text(name:'text',defaultValue:'this is text',description:'this is text param')
    
  }
  stages{
  
  stage("BUILD"){
    steps{
   bat label:'',script: 'echo build'
    }
  }
    stage("DEVOLPY"){
      steps{
        bat label:'', script:'echo devolpy'
        choice(name:'chs',choices['ios','android','pc'],description:'this is hard choice')
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
