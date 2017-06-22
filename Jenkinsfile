properties (
    [
        [
            $class  : 'jenkins.model.BuildDiscarderProperty', strategy: 
            [
                    $class      : 'LogRotator',
                    numToKeepStr: '',
                    artifactDaysToKeepStr: '90', 
                    artifactNumToKeepStr: '', 
                    daysToKeepStr: '90'
            ]
		],
        pipelineTriggers(
	        [
	        	[
	        		$class: 'TimerTrigger', spec: 'H */12 * * *'
	        	]
	        ]
		)
    ]
)

node('cloud&&centos')
{
    // print current date and time
    sh 'date'
}