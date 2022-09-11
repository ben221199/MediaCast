# Protocols

## ICY

### Version 1

- Client to Server: `password\n` or `password\r\n`
- Server to Client: 
  - `OK\n` or `OK\r\n`
  - `OK2\n` or `OK2\r\n` with following headers (e.g. `ICY-Caps: 11\n` or `ICY-Caps: 11\r\n`) and a terminating `\n` or `\r\n`.
  - Any other response will be interpreted as an error.
- Client to Server: `headerName: headerValue\n` or `headerName: headerValue\r\n` and a terminating `\n` or `\r\n`.
- Client to Server: The stream data.

### Version 2

TODO
