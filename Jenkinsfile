node('master') 
{
    stage('ContinuousDownload_Loans') 
    {
        script
        {
            try
            {
                 git 'https://github.com/intelliqittrainings/maven.git'
            }
            catch(Exception e1)
            {
                 mail bcc: '', body: 'Jenkins is unable to download the code from the git repository', cc: '', from: '', replyTo: '', subject: 'Download Failed', to: 'gitadmin@gmail.com'
                       exit(1)
            }
        }
       
    }
                 mail bcc: '', body: 'Jenkins is unable to create an artifact from the code', cc: '', from: '', replyTo: '', subject: 'Build Failed', to: 'devlopers@gmail.com' 
                      exit(1)
            }
        }
        
    }
    
    
    
    
    
}
