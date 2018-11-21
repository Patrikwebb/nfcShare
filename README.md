### Run the code

Plug your phone into your computer.

Build and run the code

    $ cd ~/nfcShare
    $ cordova run

### NFC Code
**www/js/index.js**

    var success = function () { alert("Success: NFC data sent to peer"); };
    var failure = function (reason) { alert("Sharing failed " + reason); };

    nfc.share([ndef.uriRecord("http://google.se")], success, failure);

### Share NFC information 

Open the app and hold it close to and NFC reader or another NFC device to transfer the information.