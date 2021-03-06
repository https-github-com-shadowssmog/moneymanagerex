# Anonymous Aggregate User Behaviour Analytics

Money Manager EX has begun gathering anonymous aggregate user behaviour analytics and reporting these to Google Analytics.

## Why?


## What?
Money Manager Ex's analytics record some shared information for every event:

- The Money Manager Ex user agent, e.g. ``
- The Google Analytics version, i.e. `1` (https://developers.google.com/analytics/devguides/collection/protocol/v1/parameters#v)
- The Money Manager EX analytics tracking ID, e.g. `UA-51521761-6` (https://developers.google.com/analytics/devguides/collection/protocol/v1/parameters#tid)
- A Money Manager EX analytics user ID, e.g. `1BAB65CC-FE7F-4D8C-AB45-B7DB5A6BA9CB`. This is generated by `uuidgen` and stored in the repository-specific Git configuration variable `homebrew.analyticsuuid` within `$(brew --repository)/.git/config`. This does not allow us to track individual users but does enable us to accurately measure user counts vs. event counts (https://developers.google.com/analytics/devguides/collection/protocol/v1/parameters#cid)
- The Money Manager EX application name, e.g. `MoneyManagerEx` (https://developers.google.com/analytics/devguides/collection/protocol/v1/parameters#an)
- The Money Manager EX application version, e.g. `v1.3.3` (https://developers.google.com/analytics/devguides/collection/protocol/v1/parameters#av)
