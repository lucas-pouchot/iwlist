# iwlist

parses iwlist output on linux computers. tested on raspberry pi running raspbian (debian)

@substack wrote this for [hacking into flying robots](https://github.com/substack/virus-copter/blob/master/lib/iw.js) but told me to publish it to github and npm because he was busy

## install

```javascript
npm install iwlist
```

## instantiate

```javascript
var iw = require('iwlist')('wlan0')
```

## scan(callback)

returns list of nearby wireless networks

## connect(essid, callback)

joins a wireless network by ESSID

## disconnect

disconnects from the current network. callback not implemented yet but it returns the spawned child process stream for `iwconfig`

## license

BSD LICENSED