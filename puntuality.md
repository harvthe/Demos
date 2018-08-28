# Creating accounts

`https://api.axway.training/v1/amplifyMFT/onboard`

`{
                "internal_accName":"acc1",
                "internal_passw":"password1",
                "partner_accName":"acc2",
                "partner_passw":"password2",
                "internal_subsFolder":"invoicefolder"
}`

### checking for files by APIs
`http://203.48.128.178:8080/showfiles?limit=100`
> use basic auth and the credentials you created above

## sending and receiving files

use FileZilla or other client to upload file 
`203.48.128.185`
> use basic auth and the credentials you created above

##### alternative
use the web client to upload files

[ST client](https://203.48.128.185/)
> use basic auth and the credentials you created above


create multiple account file checks through the data integration elements available in the 

07-ST-Configuration space.

Navigate to Data Integration > Routes. 

Update the 03_AccountFileChecks internal resource.

The resource content is in CSV format and should have the first line as a header.

Once you've updated your resource, navigate to Data Integration > Routes and run the  03_CreateFileChecks configuration route

From the Routes tab,  stop and restart the 01_AbsorbTrackedObject route in the 04-ST-Integration space.




