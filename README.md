# htmx "moveBefore" demo app

This is a simple website to demonstrate the new proposed `moveBefore()` functionality
available in canary chrome.

You can start the server with

```bash
$ ./server.sh
```
and then navigate to https://localhost:8000.  You will be presented with two buttons.

If you click one button it will load an iframe embed marked as [`hx-preserve`](https://htmx.org/attributes/hx-preserve/).
The site uses a customized version of htmx that uses the `moveBefore()` method for preserving elements, which
perserves things like play state.

You should be able to click back and forth between the buttons and have the video continue playing.

## Browser set up

You will need to download chrome canary:

https://www.google.com/chrome/canary/

and go to <chrome://flags/#atomic-move> and enable "Atomic DOM move" for the demo to work properly


