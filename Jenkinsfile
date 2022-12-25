pipeline 
{
    agent any

    stages {
        stage('Buid')
        {
            steps
            {
                echo 'Build Appilication'
            }
        }
         stage('Test')
        {
            steps
            {
                echo 'Test Appilication'
            }
        }
         stage('Deploy')
        {
            steps
            {
                echo 'Deploy Appilication'
            }
        }
    }
    post 
    {
        always
        {
            emailext body: 'Summary', subject: 'Pipeline Status', to: 'nagavenkatash.tatav@hcl.com,mahalakshmi.kundrapu@hcl.com'
        }
    }
}
