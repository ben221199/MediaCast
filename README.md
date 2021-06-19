# AudioCast

## Protocols

| Name | Description | Header prefix |
| -- | -- | -- |
| ICY | I Can Yell (now SHOUTcast) | `ICY-` |
| Audiocast | - | `X-Audiocast-` |
| Ice | Protocol of Icecast | `Ice-`

### ICY

| Header | Description | Value | Supported in |
| -- | -- | -- | -- |
| `ICY-BR` | **B**it **R**ate | Number | Icecast 0.8+ |
| `ICY-Name` | Name | String | Icecast 0.8+ |
| `ICY-Genre` | Genre | String | Icecast 0.8+ |
| `ICY-Notice1` | Notice 1 | String | Icecast 0.8.2+ |
| `ICY-Notice2` | Notice 2 | String | Icecast 0.8.2+ |
| `ICY-URL` | URL | Path | Icecast 0.8+ |
| `ICY-Pub` | Public | Boolean: `0` or `1` | Icecast 0.8+ |

| Header | Description | Value | Supported in |
| -- | -- | -- | -- |
| `ICY-Error` | Error | ... | Icecast 0.8+ |
| `ICY-Id` | Id | ... | Icecast 0.8+ |
| `ICY-Response` | Response | ... | Icecast 0.8+ |
| `ICY-TchFrq` | Touch Frequency | ... | Icecast 0.8+ |


| Header | Description | Value | Supported in |
| -- | -- | -- | -- |
| `ICY-Caps` | Caps | ... | Icecast 1.3.12 |
| `ICY-MetaInt` | Meta Interval | ... | Icecast 1.3.12 |
| `ICY-MetaData` | Meta Data | ... |Icecast 2.0.0 |

### Audiocast

| Header | Description | Value | Supported in |
| -- | -- | -- | -- |
| `X-Audiocast-Ack` | Acknowledge | ... | Icecast 1.3.12 |
| `X-Audiocast-Admin` | Admin | ... | Icecast 1.3.12 |
| `X-Audiocast-BitRate` | Bit Rate | ... | Icecast 1.3.12 |
| `X-Audiocast-ContentId` | Content Id | ... | Icecast 1.3.12 |
| `X-Audiocast-Description` | Description | ... | Icecast 1.3.12 |
| `X-Audiocast-Directory` | Directory | ... | Icecast 1.3.12 |
| `X-Audiocast-DumpFile` | Dump File | ... | Icecast 1.3.12 |
| `X-Audiocast-Genre` | Genre | ... | Icecast 1.3.12 |
| `X-Audiocast-Location` | Location | ... | Icecast 1.3.12 |
| `X-Audiocast-MIMEType` | MIME Type | ... | Icecast 1.3.12 |
| `X-Audiocast-Mount` | Mount | ... | Icecast 1.3.12 |
| `X-Audiocast-Name` | Name | ... | Icecast 1.3.12 |
| `X-Audiocast-Port` | Port | ... | Icecast 1.3.12 |
| `X-Audiocast-Public` | Public | ... | Icecast 1.3.12 |
| `X-Audiocast-Server-URL` | Server URL | ... | Icecast 1.3.12 |
| `X-Audiocast-StreamMsg` | Stream Message | ... | Icecast 1.3.12 |
| `X-Audiocast-StreamLength` | Stream Length | ... | Icecast 1.3.12 |
| `X-Audiocast-StreamTitle` | Stream Title | ... | Icecast 1.3.12 |
| `X-Audiocast-StreamURL` | Stream URL | ... | Icecast 1.3.12 |
| `X-Audiocast-Source-Password` | Source Password | ... | Icecast 1.3.12 |
| `X-Audiocast-Type` | Type | ... | Icecast 1.3.12 |
| `X-Audiocast-UDPPort` | UDP Port | ... | Icecast 1.3.12 |
| `X-Audiocast-UDPSeqNr` | UDP Sequence Number | ... | Icecast 1.3.12 |
| `X-Audiocast-URL` | URL | ... | Icecast 1.3.12 |
| `X-Audiocast-YP-Error` | YellowPage Error | ... | Icecast 1.3.12 |
| `X-Audiocast-YP-Id` | YellowPage Id | ... | Icecast 1.3.12 |

### Ice

| Header | Description | Value | Supported in |
| -- | -- | -- | -- |
| `Ice-Audio-Info` | Audio Info | ... | Icecast 2.0.0 |
| `Ice-BitRate` | Bit Rate | ... | Icecast 2.0.0 |
| `Ice-Description` | Description | ... | Icecast 2.0.0 |
| `Ice-Genre` | Genre | ... | Icecast 2.0.0 |
| `Ice-Name` | Name | ... | Icecast 2.0.0 |
| `Ice-Password` | Password | ... | Icecast 2.0.0 |
| `Ice-Public` | Public | ... | Icecast 2.0.0 |
| `Ice-URL` | URL | ... | Icecast 2.0.0 |
