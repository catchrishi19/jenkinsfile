#!groovy

@Library('symantec@development') _

node {

properties([buildDiscarder(logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '2', numToKeepStr: '2'))])

JAVA {
	GIT_URL 		    = 'http://10.112.78.16/Shashank/Controller-Unit-Test.git'
	GIT_CREDENTIALS 	= '8851ab4f-0fd9-4833-b5c8-64342a454278'	
	MAVEN_HOME 		    = '/usr/local/apache-maven-3.5.0'
	MAVEN_GOAL 		    = 'clean install'
	SONAR_SCANNER_HOME	= '/var/lib/jenkins/tools/hudson.plugins.sonar.SonarRunnerInstallation/sonar'
//    SONAR_PROPERTY      = '-Dsonar.scm.disabled=true -Dsonar.projectName=$BUILD_NAME -Dsonar.projectVersion=1.0 -Dsonar.sourceEncoding=UTF-8 -Dsonar.projectKey=$BUILD_ID -Dsonar.test=src/test -Dsonar.java.binaries=target/classes/net  -Dsonar.sources=src -Dsonar.projectBaseDir=/var/lib/jenkins/workspace/Sym_PipelineAsCode'

    }
}

