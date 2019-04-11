pipeline{

agent any

	stages
	{
		stage ('complie stage')
		{
			steps{
				withJDK(java : 'jdk')
				{	sh 'java -version' }

				}
		}
		
		stage ('testing stage')
		{
			steps{
				withMaven(maven : 'maven_3_6_0')
				{	sh 'mvn test' }

				}
		}
		
		stage ('deployment stage')
		{
			steps{
				withMaven(maven :'maven_3_6_0')
		
			{sh 'mvn deploy'}
		
			
				}
	}
}
}
