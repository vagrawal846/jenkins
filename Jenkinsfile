pipeline
{
    agent any 
    
    stages
    {
     
     stage ('compile code')
     {
         steps
         {
             sh 'mvn clean install'
         }
     }
     stage ('test')
     {
         steps
         {
             sh 'mvn test'
         }
     }
     stage ('find my binaryggggggg')
     {
         steps
         {
             sh 'find / -name *.war'
         }
     }
     stage ('deploy')
     {
         steps
         {
             sh 'cp -R /root/.jenkins/workspace/pipe2/target/* /opt/apache-tomcat-8.0.45/webapps'
         }
     }
        
    }
}
