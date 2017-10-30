## GET `/questions/:id`

Get a single question

```ruby--Rails
require 'rest-client'

question_id = 'PUT-YOUR-QUESTION-ID-HERE'

RestClient::Request.execute method: :get,
  url: "https://api.diduenjoy.com/api/v1/questions/#{question_id}",
  user: 'PUT-YOUR-API-KEY-HERE'
```

### attributes

attribute          | description
------------- | -------------
__position__<br>_integer_ | question position
__text__<br>_string_ | question text

### relationships

relationship          | description
------------------------------ | -------------
__survey_language__ | question survey_language
