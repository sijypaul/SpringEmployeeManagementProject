pipeline
{
    agent any
    stages 
    {
        stage('git repo & clean') 
        {
            steps
            {
              // bat "rmdir  /s /q assesmentfile"
              //bat "git clone https://github.com/sijypaul/Employee-Spring-Application.git"
               bat "mvn clean -f Employee-Spring-Application"
            }
        }
       
        stage('package')
        {
            steps 
            {
                bat "mvn package -f Employee-Spring-Application"
            }
        }
    }
}
