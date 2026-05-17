# Response Codes

## Response Parameters

|Field | Datatype | Description |
|---|---|---|
| session_start_timestamp_ms | long | The epoch timestamp in milliseconds when the session is started or revived. |
| session_end_timestamp_ms | long | The epoch timestamp in milliseconds when the session is ended. The value is null if Conviva hasn't seen the end of the session when the query is processed. |
| client_id | string | Client ID of the specific video session. The value is displayed in the format of four unsigned decimal integers separated by dots (.). |
| session_id | long | Unique identifier of a specific video session. |
| playing_time_ms | long | Total playing time in the specific video session. The value is displayed in terms of milliseconds. |
| paused_time_ms | long | The duration the player has spent in the paused state over the session's lifetime till the end of the interval. The value is displayed in milliseconds and does not include time in the long paused state. |
| session_event | array of Events | A few types of events that are related to the playback SessionStartEvent, Seek, or FatalError with the respective epoch timestamp timeMs. For example, the Player Error or Fatal exception in AVPlayer error if occurred due to the VSF (Video Start Failure) and considered as a FatalError. |
| cdn	| array of States | The name of the content delivery networks from which the device was receiving video data. It shows the collection of session epoch timestamp startTimeMs and endTimeMs associated to the content delivery networks (CDNs) (for example, AKAMAI, FIRSTLY, CLOUDFLARE). |



## HTTP Codes 
| Status Code | Description |
|---|---|
| 200 | Success |
| 400 | Invalid request |
| 401 | Unauthorized |
| 404 | Not found |
