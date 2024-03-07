
# HOW TO RUN TEST SCRIPTS IN THIS FOLDER
- Start terminal at this folder
- Run cmd: jmeter -q dev.properties
- Command above will start JMeter GUI with predefined properties in dev.properties

## Run this query for ES 7 after execute Create subscription script
```json
POST notification_message_subscription/_delete_by_query
{
  "query": {
    "wildcard": {
      "userEmail.keyword": {
        "value": "user-benchmark-*"
      }
    }
  }
}
```
