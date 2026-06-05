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