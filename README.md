#Swift Monitoring : Nagios 

This repo contains script for Monitoring of Openstack-Swift. This could be used by Nagios over NRPE to get the status of Swift Installation.

## Usage
    

   Usage : 

                       '-a', '--authURL',   required=True,
                       help="Auth URL for getting the auth token ")
                       
                       '-u', '--username',  required=True,
                       help="Username for getting the auth token ")
                       
                       '-k', '--key',       required=True,
                       help="Password for the user for getting auth token")
                       
                       '-x', '--tenant',    required=True,
                       help="tenant name for getting auth token")
                       
                       '-c', '--container', default='check_swift',
                       help="name of container to upload")
                       
		       '-s', '--sizemax',   default='1024', type=int,
                       help="max sized file to be uploaded"


    OUTPUT :  
    
			Returns four states under following conditions
    			STATE_OK : When upload+download+delete commands work fine
    			STATE_UNKNOWN : Swift command not found/not installed
    			STATE_WARNING : Swift Seems fine, problem with this script
    			STATE_CRITICAL: Swift has problmes uploading/downloading/deleting '''
