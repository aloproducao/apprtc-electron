# AppRTC Demo for electron

This demo is electron for apprtc（https://appr.tc/）。
sourcecode ： https://github.com/webrtc/apprtc

＃ How to use

```
# Clone this repository
git clone https://github.com/daozhao/apprtc-electron.git
cd apprtc-electron
npm install
npm start
```

# How to change self server

open appwindow.js,

```
//change server address.
var roomServer = 'https://appr.tc';
```

if  your server is self certificate 
```
// add this code to main.js
app.on('certificate-error', (event, webContents, url, error, certificate, callback) => {
      event.preventDefault()
      callback(true)
  })
```
