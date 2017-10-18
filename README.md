# Hello Phoenix Chat

Demonstration chat app built in Phoenix 1.3.0 from [Phoenix Guides](https://hexdocs.pm/phoenix/channels.html#tying-it-all-together).

- [x] Channels Sample application [
    [guide](https://hexdocs.pm/phoenix/channels.html#tying-it-all-together) |
    [code](https://github.com/smeade/phoenixchat) |
    [demo](http://phx-009-channels.herokuapp.com/)
    ]
  - [x] uncomment the “room:*” channel definition [
    [code](https://github.com/smeade/phoenixchat/blob/master/lib/hello_web/channels/user_socket.ex#L5)
    ]
  - [x] define a HelloWeb.RoomChannel module [
    [code](https://github.com/smeade/phoenixchat/blob/master/lib/hello_web/channels/room_channel.ex)
    ]
  - [x] Joining Channels [[guide](https://hexdocs.pm/phoenix/channels.html#joining-channels)]
    - [x] authorize clients to join topic [
      [code](https://github.com/smeade/phoenixchat/blob/master/lib/hello_web/channels/room_channel.ex#L4-L9)
      ]
    - [x] set our room name to “room:lobby” [
      [code](https://github.com/smeade/phoenixchat/blob/master/assets/js/socket.js#L57)
      ]
    - [x] join channel [
      [code](https://github.com/smeade/phoenixchat/blob/master/assets/js/socket.js#L79-L81)
      ]
    - [x] import assets/js/socket.js [
      [code](https://github.com/smeade/phoenixchat/blob/master/assets/js/app.js#L21)
      ]
    - [x] add containers to hold our chat messages [
      [code](https://github.com/smeade/phoenixchat/blob/master/lib/hello_web/templates/page/index.html.eex#L12-L14)
      ]
    - [x] push an event over the channel with the message body [
      [code](https://github.com/smeade/phoenixchat/blob/master/assets/js/socket.js#L64-L70)
      ]
    - [x] listen for new messages and append them to our messages container [
      [code](https://github.com/smeade/phoenixchat/blob/master/assets/js/socket.js#L64-L70)
      ]
  - [x] Handle Incoming Events [
    [guide](https://hexdocs.pm/phoenix/channels.html#incoming-events) |
    [code](https://github.com/smeade/phoenixchat/blob/master/lib/hello_web/channels/room_channel.ex#L11-L14)
    ]
