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
              bat "git clone https://github.com/sijypaul/SpringEmployeeManagementProject.git"
               bat "mvn clean -f SpringEmployeeManagementProject"
            }
        }
       
        stage('package')
        {
            steps 
            {
                bat "mvn package -f SpringEmployeeManagementProject"
            }
        }
    }
}
