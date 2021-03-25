## SSE with Flask

Have a look at Server-Sent Events. Server-Sent Events is a browser API that lets you keep open a socket to your server, subscribing to a stream of updates. For more Information read Alex MacCaw (Author of Juggernaut) post on why he kills juggernaut and why the simpler Server-Sent Events are in manny cases the better tool for the job than Websockets.

The protocol is really easy. Just add the mimetype text/event-stream to your response. The browser will keep the connection open and listen for updates. An Event sent from the server is a line of text starting with data: and a following newline.

##### This is useful for real time updates to frontend, eg Iot dashboards

#### Install requirements and Run,

`python app.py`