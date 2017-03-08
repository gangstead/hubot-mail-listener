# hubot-mail-listener

hubot-mail-listener adds an **IMAP** listener plugin to hubot that reports
unread or incoming new emails (sender, subject, date, text message).

Message is put in as a slack message attachment

![demo](https://raw.githubusercontent.com/gangstead/hubot-mail-listener/master/demo.png)

## Installation

Edit the `package.json` for your hubot and add the hubot-mail-listener
dependency.

```javascript
"dependencies": {
  "hubot-mail-listener": ">= 0.0.1",
  ...
}
```

## Configuration

The following variables are required to let the script work:

* `HUBOT_MAIL_LISTENER_ROOMS`, comma separated list of rooms where incoming emails should be posted
* `HUBOT_MAIL_LISTENER_USERNAME`, username
* `HUBOT_MAIL_LISTENER_PASSWORD`, password
* `HUBOT_MAIL_LISTENER_HOST`, mail host

The following variables are optional:

* `HUBOT_MAIL_LISTENER_PORT`, mail host port, default to `993`
* `HUBOT_MAIL_LISTENER_SECURE`, whether to use secure connection, default to `true`
* `HUBOT_MAIL_LISTENER_MAILBOX`, mail box to monitor, default to `INBOX`
* `HUBOT_MAIL_LISTENER_MARK_SEEN`, whether to mark seen email as read, default to `true`
* `HUBOT_MAIL_LISTENER_FETCH_UNREAD`, whether to fetch unread emails on start, default to `true`

## See Also

This work is an updated and coffeescript free version of: https://github.com/matteoagosti/hubot-mail-notifier
