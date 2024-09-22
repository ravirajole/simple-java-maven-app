pipeline
{
 agent any
 stages
 {
  stage('scm checkout')
  { steps { git 'https://github.com/ravirajole/simple-java-maven-app.git'}  }

  stage('build the code')    //build the job
  { steps { withMaven(globalMavenSettingsConfig: '', jdk: 'JDK_Home', maven: 'MVN_home', mavenSettingsConfig: '', traceability: true) 
	    { sh 'mvn package'} }  
  }
 }
}
