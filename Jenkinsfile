pipeline 
{
    agent any

    stages 
    {
        stage('Build') 
        {
            steps 
            {
                echo 'Build Application'
            }
        }

         stage('Test') 
        {
            steps 
            {
                echo 'Test Application'
            }
        }

         stage('Deploy') 
        {
            steps 
            {
                echo 'Deploy Application'
            }
        }
    }

    post 
    {
        
        always 
        {
            emailext body: 'Build Succeded', subject: 'Pipeline Status', to: 'rajutrainings123@gmail.com'
        }
    }
}
