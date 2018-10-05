# js_worker
If there will be an error:`Failed to construct 'Worker': Script at 'file:///path/worker.js' cannot be accessed from origin 'null'.
`
That's because, for some good security reasons, Chrome doesn't let you load web workers when running scripts from a local file.
Here are two ways to resolve:
1. close all chrome tabs, open terminal, `/Applications/Google\ Chrome.app/ts/MacOS/Google\ Chrome --allow-file-access-from-files`
2. install [web server for chrome](https://chrome.google.com/webstore/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb?hl=en)
