###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_ReadLE64

Use this function to read 64 bits of little-endian data from an [SDL_RWops](SDL_RWops) and return in native format.

## Syntax

```c
Uint64 SDL_ReadLE64(SDL_RWops * src);

```

## Function Parameters

|             |                                    |
| ----------- | ---------------------------------- |
| **src**     | the stream from which to read data |

## Return Value

Returns 64 bits of data in the native byte order of the platform.

## Remarks

SDL byteswaps the data only if necessary, so the data returned will be in
the native byte order.

## Version

This function is available since SDL 3.0.0.

## Related Functions

* [SDL_ReadBE64](SDL_ReadBE64)

----
[CategoryAPI](CategoryAPI), [CategoryIO](CategoryIO)


