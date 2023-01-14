pipeline{
    agent any
    stages{
            stage("Source Code Checkout"){
               steps{
                git branch: 'main', url: 'https://github.com/ullahjunaid/Question-2.git'                }  
            
            }
             stage("Shubam's 2 stage"){
                when{
                    expression {
                        
                       params.Build_Number== true
                   }
                }
                steps{
                    echo  "This is 2nd stage "
                }
            }
              stage("Shubam's 3rd stage"){
                steps{
                    echo  "This is stage will 3rd stage"   
                }
            }
            
         }
}