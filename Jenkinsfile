pipeline 
{
    agent any 
  //{
    //    label 'Build2'
    //}

    stages {
        stage('Checkout') {
            steps {
          checkout scmGit(branches: [[name: '*/master']], browser: github('https://github.com/Jayparmar98/flowershop-demo-aspdotnet'), extensions: [], userRemoteConfigs: [[credentialsId: 'Git-Token', url: 'https://github.com/Jayparmar98/flowershop-demo-aspdotnet.git']])
          bat "dir"
        
                  }
       // }
         //stage('Build') {
           // steps {
             //      bat 'dotnet build asp.net.sln'
               //   }
             
         //}
        //stage('publish') {
         //   steps {
           //        bat 'dotnet publish asp.net.sln'
             //     }
        //}
         //stage('Zip') {
           // steps { 
            //bat "powershell compress-Archive -Path C:\\Node\\workspace\\win_build\\asp.net\\bin\\Debug\\net6.0\\publish\\* -DestinationPath ${WORKSPACE}\\Nuget-ID-${BUILD_ID}-Date-${BUILD_TIMESTAMP}.zip"
            //}
        //}
         //stage('Artifacts') {
           // steps { 
            //nexusArtifactUploader artifacts: [[artifactId: 'Artifacts', classifier: '${BUILD_TIMESTAMP}', file: 'Nuget-ID-${BUILD_ID}-Date-${BUILD_TIMESTAMP}.zip', type: 'zip']], credentialsId: 'NEXUS', groupId: 'Dotnet', nexusUrl: '102.37.21.132:8081', nexusVersion: 'nexus3', protocol: 'http', repository: 'Nuget', version: '1.1'
            //}
        //}
    //stage('Deploy') {
      //     agent { 
        //    label 'Master'
          //       }
            //steps { 
            //sh 'ansible-playbook /etc/ansible/latest.yml'
            //}
        //}
        
    }
}    
