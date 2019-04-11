pipeline{

agent any

	stages
	{
		stage ('complie stage')
		{
			steps{
				withMaven(maven : 'maven_3_6_0')
				{	sh 'mvn clean compile' }

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
