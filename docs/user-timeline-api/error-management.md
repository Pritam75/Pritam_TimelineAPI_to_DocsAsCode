# HTTP Response Codes

## 200: Success
Successful execution of this API request is represented by the response code 200.

### Request
Query with a valid user_id, session_id, or both.
For example, 
- v2/validation-timeline?user_id={“12345678”}&session_id={“-923452232”}
- v2/validation-timeline?session_id={“-923452232”}
- v2/validation-timeline?user_id={“12345678”}

### Response
Fetch the session summaries, event timelines, and metadata in JSON format for the given user_id and/or session_id.


## 4xx: Client-side Errors
Client-side error codes start with the number 4, for example, 400 (Bad Request), 401 (Unauthorized), 404 (Not Found).

### Request
Query with only NULL session_id
For example:
v2/validation-timeline?session_id={null}

### Response
417 - Exception Failed
Please pass a valid 'user_id'/'session_id' or both in the request URL.


## 5xx: Server-side Errors

### Request
Query with an invalid user_id.
For example:
v2/validation-timeline?user_id={“123”}&session_id={“611122020”}

### Response
503 - Service Unavailable
Error: No record found for invalid userId: 123 and sessionId: 611122020. Try again with a valid userID. If the issue continues, contact ABC Support.


### Request
Query with an invalid session_id.
For example:
v2/validation-timeline?user_id={“12345678”}&session_id={“123”}

### Response
503 - Service Unavailable
Error: No record found for userId: 12345678 and invalid sessionId: 123. Try again with a valid sessionID. If the issue continues, contact ABC Support.


