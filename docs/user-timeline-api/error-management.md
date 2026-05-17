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

