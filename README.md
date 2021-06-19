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
| `ICY-URL` | **U**niform **R**esource **L**ocator | Path | Icecast 0.8+ |
| `ICY-Pub` | Public | Boolean: `0` or `1` | Icecast 0.8+ |

| Header | Description | Value | Supported in |
| -- | -- | -- | -- |
| `ICY-Error` | Error | ... | Icecast 0.8+ |
| `ICY-Id` | Id | ... | Icecast 0.8+ |
| `ICY-Response` | Response | ... | Icecast 0.8+ |
| `ICY-TchFrq` | Touch Frequency | ... | Icecast 0.8+ |


### Audiocast

_TODO_

### Ice

_TODO_
