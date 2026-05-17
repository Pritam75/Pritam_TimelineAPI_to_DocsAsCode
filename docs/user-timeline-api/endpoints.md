# API Endpoints

## Retrieve User Timeline Data

### Query with the combination of a valid user_id and session_id
Retrieves the session summaries, event timelines, and metadata of a particular user’s session.
```http
https://api.<companyName>/validation/<version>/timeline?user_id={value}&session_id={value}
```

### Query with only a valid session_id
Retrieves the session summaries, event timelines, and metadata of a particular user's session.
```http
https://api.<companyName>/validation/<version>/timeline?session_id={value}
```

### Query with only a valid user_id
Retrieves the session summaries, event timelines, and metadata of the latest user’s session.
```http
https://api.<companyName>/validation/<version>/timeline?user_id={value}
```
