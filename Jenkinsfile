pipeline
{
  agent any
  parameters{
    string (name:'str',defaultValue:'default',description:'this is string param')
    booleanParam(name:'bool',defaultValue:'default',description:'this is bool param')
    text(name:'text',defaultValue:'this is text',description:'this is text param')
     choice(
      description: '你需要选择哪个模块进行构建 ?',
      name: 'modulename',
      choices: ['ios', 'android', 'Module3']
    )
  }
  stages{
  
  stage("BUILD"){
    steps{
      bat label:'',script: 'echo build'
      bat label:'',script:'echo ${param.bool}'
       bat label:'',script:'echo ${param.str}'
       bat label:'',script:'echo ${param.text}'
       bat label:'',script:'echo ${param.modulename}'
      
    }
  }
    stage("DEVOLPY"){
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
