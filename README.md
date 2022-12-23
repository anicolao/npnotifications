# Neptune's Pride Notifications

To use this repo, clone it and grep for `REPLACE` and replace all
the personal information.

You'll need a pushover api key, a pushover user key, a neptune's
pride game id and alias, and a neptune's pride API key.

Once you've replaced all those try out

./checkattacks

Finally add checkattacks to crontab.

The convention is to put your NP API as the name used everywhere;
in the repo as it stands it is set to "Anne" the last alias I was
using on NP. The idea being you can have many instances of these
files, one for each game you are sending notifications to, and many
crontab entries on different schedules corresponding to the game
ticks.

The game ticks aren't always perfectly on time, so you have to
schedule your cron job for a minute or two later. On 1h ticks, I'd
go for 5 minutes after tick time as a nice large, safe buffer.
