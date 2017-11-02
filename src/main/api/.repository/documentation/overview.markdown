##**PRIMO Notifications API Overview**

***
> **`Purpose of API`**    - The purpose of this API is to deal with notification(s) related to User 

***

**`Below are the operations supported by this API  `**

>**`GET`**   -   
1. Retrieve Notifications list 
2. Retrieve Notification details as per the schema definations based on Notification Id supplied as an URI parameters

***

>**`PUT`**   - 
Update a Notification . The Client system needs to pass the values as per the schema and it will update Records for a specific notifications. 

***

>**`POST`**  - 
Create a Notification . The Client system needs to pass the values as per the schema and it will Create resource for notification. 

***

##**API End Point**
 Is this section required ?
 
> Notifications API has End Point residing on Mainframe CICS. 
  
>      'http://dktopm01.topdanmark.local:07564/cics/services/notification/{version}/notifications'
 **API Version - {version}**                                           | **Functionality** 
  ------------                                                         | -------------
  v1                                                                   | Deals with GET,PUT,POST
  vn                                                                   | New Capabality


##**Authentication**
> Notifications API has been secured by SessionId and to perform any HTTP methods it requires X-PTS-SESSIONID 

>      'X-PTS-SESSIONID': '000000000B009549887288392960476031591586021C6000020000000000'


##**Error Code** (Is this section required ?)
Error Codes that can be returned by any method.

  **Error Code**                                                       | **Description** 
  ------------                                                         | -------------
                                                                       | Ok
                                                                       | Bad request
                                                                       | No action was requested
                                                                       | The requested class does not exist
                                                                       | Authentication failed
                                                                       | Object not found
                                                                       | Property is invalid
                                                                       | A data validation error has occurred
                                                                       | Method Not Implemented
                                                                       | Permission denied
                                                                       | API rate limit exceeded

