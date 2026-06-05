# Troubleshooting Scenarios



## Client Removed from Domain

### Issue

 Client could not log into domain account

### Diagnosis

 Verified machine no longer belonged to domain.


 ### Resolution

 Removed and rejoined domain.


 ### Result 

 Authentication restored

![Client not listed under computers](media/domain-knockoff.png)
 &ensp;
&ensp;
Notice the client computer is not listed under the domain
 &ensp;
 &ensp;
![Client can't log into due to domain knockoff](media/domain-knockoff-client-msg.png)
And user cannot log into due to broken trust relationship (computer knocked off from domain)
 &ensp;
 &ensp;
![Logging in as admin on client computer](media/rejoining-domain-1.png)
Log into admin account on client computer, navigate to System >> About >> Domain and services
 &ensp;
 &ensp;
![Rejoining domain](media/rejoining-domain-2.png)
&ensp;
 &ensp;
Type the name of computer to rejoin that computer to domain then click "Network ID" and follow the prompt. Admin password is needed.

Domain Rejoined (Server)

![Domain Rejoined](media/domain-reattached.png)

 &ensp;


 &ensp;&ensp;&ensp;&ensp;

## DNS Resolution Failure

### Issue
`ping kevtech.com` failed


### Diagnosis

Incorrect network adapter configuration. 


### Resolution

Changed client adapter from Bridged to Host-Only.


### Result

Successful domain communication.