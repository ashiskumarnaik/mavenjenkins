pipeline 
{
    agent any 

    stages
    {
        stage ('Hello')
        {
            steps{
            echo 'Hello World'
            }
        }
        stage ('Build')
        {
            steps {
            echo 'Build App'
            }
        }
        stage ('Test')
        {
            steps {
            echo 'Test App'
            }
        }
        stage ('Deploy')
        {
            steps {
            echo 'Deploy App'
            }
        }

    }
    post 
    {
        always 
        {
            emailext body: 'summary', subject: 'pipeline status', to: 'ashishami2002@gmail.com'
        }

    }
}
