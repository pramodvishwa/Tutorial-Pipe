#!groovy
@Library('GlobaLPipeline@master') _
node {
    properties([buildDiscarder(logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '2', numToKeepStr: '2'))])
    Pipeline_as_code {
        GIT_URL                 = 'https://github.com/pramodvishwa/Tutorial-Pipe.git'
	BRANCH			= 'dev'
        GIT_CREDENTIALS         = 'Git-Credentials'
	MAVEN_HOME		= '/app/apache-maven/'
        MAVEN_GOAL		= 'clean install'
	MVN_SKIP_GOAL		= 'clean install DskipTests=true'
	SONAR_PROPERTY		= 'sonar-project.properties'
        RECIPIENT               = 'pramod.s.02@gmail.com'
        EMAIL_TEMPLATE          = 'email_template'
    }
}

