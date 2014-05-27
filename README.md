Slackbot
========
Slackbot wrapper for [slack.com](https://slack.com)


## Install

    % npm install slackbot

add slackbot integration and get `token`

- https://YOUR-TEAM.slack.com/services/new/slackbot


## Usage

```javascript
var Slackbot = require('slackbot')

var slackbot = new Slackbot('YOUR-TEAM', 'YOUR-TOKEN');

slackbot.send("#general", "hello!!", function(err, res, body) {
  if(err) return;
  console.log(body);
});
```


## Sample

    % SLACK_TEAM=teamname SLACK_TOKEN=a1b2cdef345 node sample.js "hello world"


## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

