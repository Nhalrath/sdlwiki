# Log Handling

'''Include File(s):'''  [http://hg.libsdl.org/SDL/file/default/include/SDL_log.h SDL_log.h]


## Introduction

This category contains functions for handling simple log messages with categories and priorities.

<<Include(SDL_LogPriority, , , from="Start Include Default Priority", to="## End Include Default Priority")>>

If you're debugging SDL you might want to call:
 '''SDL_LogSetAllPriority(SDL_LOG_PRIORITY_VERBOSE);'''

Here's where the messages go on different platforms:
{|
|Windows
|debug output stream
|-
|Android
|log output
|-
|PSP
|"SDL_Log.txt"
|-
|Others
|standard error output (stderr)
|}

Messages longer than the maximum size (4096 bytes) will be truncated.


## Enumerations
<<FullSearchCached(category:CategoryEnum CategoryLog -title:SGEnumerations)>>

<!-- #Remove this line and the ## below to use this markup if it becomes relevant to this category -->
<!-- #== Structures == -->
<!-- #<<FullSearchCached(category:CategoryStruct CategoryLog -title:SGStructures)>> -->

## Functions
<<FullSearchCached(category:CategoryLog -CategoryEnum -CategoryStruct -title:SGFunctions)>>

<!-- BEGIN CATEGORY LIST -->
- [SDL_Log](SDL_Log)
- [SDL_LOG_CATEGORY](SDL_LOG_CATEGORY)
- [SDL_LogCritical](SDL_LogCritical)
- [SDL_LogDebug](SDL_LogDebug)
- [SDL_LogError](SDL_LogError)
- [SDL_LogGetOutputFunction](SDL_LogGetOutputFunction)
- [SDL_LogGetPriority](SDL_LogGetPriority)
- [SDL_LogInfo](SDL_LogInfo)
- [SDL_LogMessage](SDL_LogMessage)
- [SDL_LogMessageV](SDL_LogMessageV)
- [SDL_LogPriority](SDL_LogPriority)
- [SDL_LogResetPriorities](SDL_LogResetPriorities)
- [SDL_LogSetAllPriority](SDL_LogSetAllPriority)
- [SDL_LogSetOutputFunction](SDL_LogSetOutputFunction)
- [SDL_LogSetPriority](SDL_LogSetPriority)
- [SDL_LogVerbose](SDL_LogVerbose)
- [SDL_LogWarn](SDL_LogWarn)
<!-- END CATEGORY LIST -->
----
CategoryCategory
