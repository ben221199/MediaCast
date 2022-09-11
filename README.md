# MediaCast

## Protocol Headers

| Name | Description | Header prefix |
| -- | -- | -- |
| ICY | I Can Yell (now SHOUTcast) | `ICY-` |
| Audiocast | - | `X-Audiocast-` |
| Ice | Protocol of Icecast | `Ice-`

### ICY

| Header | Description | Value | Supported in |
| -- | -- | -- | -- |
| `ICY-BR` | **B**it **R**ate | Number | Icecast 0.8 - Icecast 2.4.99.2 |
| `ICY-Caps` | Caps | ... | Icecast 1.3 - Icecast 1.3.12 |
| `ICY-Description` | Description | ... | Icecast 2.3.0 - Icecast 2.4.99.2 |
| `ICY-Error` | Error | ... | Icecast 0.8 - Icecast 1.3.9 |
| `ICY-Genre` | Genre | String | Icecast 0.8 - Icecast 2.4.99.2 |
| `ICY-Id` | Id | ... | Icecast 0.8 - Icecast 1.3.9 |
| `ICY-MetaData` | Meta Data | ... | Icecast 2.0 Beta 1<br>Icecast 2.0.0 - Icecast 2.4.99.2 |
| `ICY-MetaInt` | Meta Interval | ... | Icecast 1.3 - Icecast 2.4.99.2 |
| `ICY-Name` | Name | String | Icecast 0.8 - Icecast 2.4.99.2 |
| `ICY-Notice1` | Notice 1 | String |  Icecast 0.8.2+ (only mentioned)<br>Icecast 1.3 - Icecast 1.3.12 |
| `ICY-Notice2` | Notice 2 | String | Icecast 0.8.2+ (only mentioned)<br>Icecast 1.3 - Icecast 1.3.12 |
| `ICY-Pub` | Public | Boolean: `0` or `1` | Icecast 1.3 - Icecast 2.4.99.2 |
| `ICY-Public` | Public | Boolean: `0` or `1` | Icecast 2.1 - Icecast 2.4.99.2 |
| `ICY-Response` | Response | ... | Icecast 0.8 - Icecast 1.3.9 |
| `ICY-TchFrq` | Touch Frequency | ... | Icecast 0.8 - Icecast 1.3.9 |
| `ICY-URL` | URL | Path | Icecast 0.8 - Icecast 2.4.99.2 |

Note: In Icecast, all the headers are lowercase. In fact, HTTP headers should be case-insensitive, but using uppercase can give problems in older releases in Icecast.

### Audiocast

| Header | Description | Value | Supported in |
| -- | -- | -- | -- |
| `X-Audiocast-Ack` | Acknowledge | ... | Icecast 1.3.5 - Icecast 1.3.12 |
| `X-Audiocast-Admin` | Admin | ... | Icecast 1.3 - Icecast 1.3.12 |
| `X-Audiocast-BitRate` | Bit Rate | ... | Icecast 1.1.4 - Icecast 1.3.12<br>Icecast 2.3.0 - Icecast 2.4.99.2 |
| `X-Audiocast-ContentId` | Content Id | ... | Icecast 1.3.5 - Icecast 1.3.12 |
| `X-Audiocast-Description` | Description | ... | Icecast 1.1.4 - Icecast 1.3.12<br>Icecast 2.3.0 - Icecast 2.4.99.2 |
| `X-Audiocast-Directory` | Directory | ... | Icecast 1.3 - Icecast 1.3.12 |
| `X-Audiocast-DumpFile` | Dump File | ... | Icecast 1.3 - Icecast 1.3.12 |
| `X-Audiocast-Genre` | Genre | ... | Icecast 1.1.4 - Icecast 1.3.12<br>Icecast 2.3.0 - Icecast 2.4.99.2 |
| `X-Audiocast-Location` | Location | ... | Icecast 1.3 - Icecast 1.3.12 |
| `X-Audiocast-MIMEType` | MIME Type | ... | Icecast 1.3.5 - Icecast 1.3.12 |
| `X-Audiocast-Mount` | Mount | ... | Icecast 1.3 - Icecast 1.3.12 |
| `X-Audiocast-Name` | Name | ... | Icecast 1.1.4 - Icecast 1.3.12<br>Icecast 2.3.0 - Icecast 2.4.99.2 |
| `X-Audiocast-Port` | Port | ... | Icecast 1.3.5 - Icecast 1.3.12 |
| `X-Audiocast-Public` | Public | ... | Icecast 1.1.4 - Icecast 1.3.12<br>Icecast 2.3.0 - Icecast 2.4.99.2 |
| `X-Audiocast-Server-URL` | Server URL | ... | Icecast 1.3 - Icecast 1.3.12 |
| `X-Audiocast-StreamMsg` | Stream Message | ... | Icecast 1.3.5 - Icecast 1.3.12 |
| `X-Audiocast-StreamLength` | Stream Length | ... | Icecast 1.3.5 - Icecast 1.3.12 |
| `X-Audiocast-StreamTitle` | Stream Title | ... | Icecast 1.3 - Icecast 1.3.12 |
| `X-Audiocast-StreamURL` | Stream URL | ... | Icecast 1.3 - Icecast 1.3.12 |
| `X-Audiocast-Source-Password` | Source Password | ... | Icecast 1.3.5 - Icecast 1.3.12 |
| `X-Audiocast-Type` | Type | ... | Icecast 1.3 - Icecast 1.3.12 |
| `X-Audiocast-UDPPort` | UDP Port | ... | Icecast 1.3 - Icecast 1.3.12 |
| `X-Audiocast-UDPSeqNr` | UDP Sequence Number | ... | Icecast 1.3.5 - Icecast 1.3.12 |
| `X-Audiocast-URL` | URL | ... | Icecast 1.1.4 - Icecast 1.3.12<br>Icecast 2.3.0 - Icecast 2.4.99.2 |
| `X-Audiocast-YP-Error` | YellowPage Error | ... | Icecast 1.3 - Icecast 1.3.12 |
| `X-Audiocast-YP-Id` | YellowPage Id | ... | Icecast 1.3 - Icecast 1.3.12 |

Note: In Icecast, all the headers are lowercase. In fact, HTTP headers should be case-insensitive, but using uppercase can give problems in older releases in Icecast.

### Ice

| Header | Description | Value | Supported in |
| -- | -- | -- | -- |
| `Ice-Audio-Info` | Audio Info | ... | Icecast 2.0 Beta 1<br>Icecast 2.0.0 - Icecast 2.4.99.2 |
| `Ice-BitRate` | Bit Rate | ... | Icecast 2.0 Beta 1<br>Icecast 2.0.0 - Icecast 2.4.99.2 |
| `Ice-Description` | Description | ... | Icecast 2.0 Beta 1<br>Icecast 2.0.0 - Icecast 2.4.99.2 |
| `Ice-Genre` | Genre | ... | Icecast 2.0 Beta 1<br>Icecast 2.0.0 - Icecast 2.4.99.2 |
| `Ice-Name` | Name | ... | Icecast 2.0 Beta 1<br>Icecast 2.0.0 - Icecast 2.4.99.2 |
| `Ice-Password` | Password | ... | Icecast 2.0 Beta 1<br>Icecast 2.0.0 - Icecast 2.4.99.2 |
| `Ice-Public` | Public | ... | Icecast 2.0 Beta 1<br>Icecast 2.0.0 - Icecast 2.4.99.2 |
| `Ice-URL` | URL | ... | Icecast 2.0 Beta 1<br>Icecast 2.0.0 - Icecast 2.4.99.2 |

Note: In Icecast, all the headers are lowercase. In fact, HTTP headers should be case-insensitive, but using uppercase can give problems in older releases in Icecast.
