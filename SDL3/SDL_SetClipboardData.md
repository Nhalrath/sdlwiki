###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_SetClipboardData

Offer clipboard data to the OS 

## Syntax

```c
int SDL_SetClipboardData(SDL_ClipboardDataCallback callback, size_t mime_count,
                         const char **mime_types, void *userdata);

```

## Function Parameters

|                    |                                                                     |
| ------------------ | ------------------------------------------------------------------- |
| **callback**       | A function pointer to the function that provides the clipboard data |
| **mime_count**     | The number of mime-types in the mime_types list                     |
| **mime_types**     | A list of mime-types that are being offered                         |
| **userdata**       | An opaque pointer that will be forwarded to the callback            |

## Return Value

Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Tell the operating system that the application is offering clipboard data
for each of the proivded mime-types. Once another application requests the
data the callback function will be called allowing it to generate and
respond with the data for the requested mime-type.

The userdata submitted to this function needs to be freed manually. The
following scenarios need to be handled:

- When the programs clipboard is replaced (cancelled)
  [SDL_EVENT_CLIPBOARD_CANCELLED](SDL_EVENT_CLIPBOARD_CANCELLED)
- Before calling [SDL_Quit](SDL_Quit)()

## Version

This function is available since SDL 3.0.0.

## Related Functions

* [SDL_ClipboardDataCallback](SDL_ClipboardDataCallback)
* [SDL_GetClipboardUserdata](SDL_GetClipboardUserdata)
* [SDL_SetClipboardData](SDL_SetClipboardData)
* [SDL_GetClipboardData](SDL_GetClipboardData)
* [SDL_HasClipboardData](SDL_HasClipboardData)

----
[CategoryAPI](CategoryAPI)

