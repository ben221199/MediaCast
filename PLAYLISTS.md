# Playlists

## M3U / M3U8

TODO

## PLS

The extension **PLS** stands for "<ins>**P**</ins>lay<ins>**l**</ins>i<ins>**s**</ins>t".
The PLS file has the same format as the INI file,

### Versions

| Name | Developer | Software |
| -- | -- | -- |
| PLSv1 (PLS) | codeArts | museArc |
| PLSv2 | NullSoft | SHOUTcast |

### Directives

All directives are case-sensitive.

| Directive | Type | Description | Supported in version 1 | Supported in version 2 | Value | Example |
| -- | -- | -- | -- | -- | -- | -- |
| `[playlist]` | Section | Section that tells that the file is a playlist. All directives are under this section. | ✅ | ✅ | - | `[playlist]` |
| `NumberOfEntries` | Property | Property that shows the amount of entries in the playlist. | ✅ | ✅ | 0 or positive integer | `NumberOfEntries=45` |
| `File#` where `#` is positive integer | Property | Property that shows the path of the entry. It differs in version 1 and version 2. | ✅ | ✅ | See [path](#path). | `File24=C:\Users\Test\Music\example.mp3` |
| `Title#` where `#` is positive integer | Property | Property that shows the title of the entry. | ❌ | ✅ | String | `Title24=Title of the Example Track` |
| `Length#` where `#` is positive integer | Property | Property that shows the length of the entry in seconds. | ❌ | ✅ | String | `Length24=62` |
| `Version` | Property | Property that shows the version of the PLS file. Because there are only 2 versions and `Version` isn't supported in PLSv1, the only value that is possible at the moment, is `2`. | ❌ | ✅ | `2` | `Version=2` |

### Path

#### Version 1

In version 1, the path can be just a path, but there are also some additional properties. This properties are seperated by a `;` so both the path as the additional properties cannot have a `;` in its value. It seems that all properties are optional, so leaving out the trailing ones, shouldn't give any trouble.
The total format is like this: `path;title;volume;duration`, and all positibilities:
 - `path;title;volume;duration`
 - `path;title;volume`
 - `path;title`
 - `path`

The `path` is just the path without any `;`, `title` is the title of the track without any `;`, `volume` is an integer between 1 and 100, and `duration` is the playback duration of the track in miliseconds.

An example:
`File24=C:\Users\Test\Music\example.mp3;Title of the Example Track;75;62000`

#### Version 2

In version 2, it is just the path to the file without additional properties. It can be a local relative, absolute or remote file, both in Windows or Unix format, depending on your OS.
