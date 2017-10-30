## GET `/surveys`

List all your surveys

```ruby--Rails
require 'rest-client'

RestClient::Request.execute method: :get,
  url: 'https://api.diduenjoy.com/api/v1/surveys',
  user: 'PUT-YOUR-API-KEY-HERE'
```

### attributes

attribute          | description
------------- | -------------
__created_at__<br>_datetime_  | survey creation date
__updated_at__<br>_datetime_  | survey last modification date
__name__<br>_string_  | survey name
__hash__<br>_string_  | survey public hash, used with companies custom mailing systems

### relationships

relationship          |description
------------------------------ | -------------
__company__  | company owning the survey
__survey_languages__  | survey localized texts (at least 1)