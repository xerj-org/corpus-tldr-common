# adb logcat

> Dump a log of system messages.
> More information: <https://developer.android.com/tools/logcat>.

- Display system logs:

`adb logcat`

- Display lines that match a `regex`:

`adb logcat -e {{regex}}`

- Display logs for a tag in a specific mode (Verbose, Debug, Info, Warning, Error, Fatal, Silent), filtering other tags:

`adb logcat {{tag}}:{{mode}} *:S`

- Display logs for React Native applications in Verbose mode Silencing other tags:

`adb logcat ReactNative:V ReactNativeJS:V *:S`

- Display logs for all tags with priority level Warning and higher:

`adb logcat *:W`

- Display logs for a specific PID:

`adb logcat --pid {{process_id}}`

- Display logs for the process of a specific package:

`adb logcat --pid $(adb shell pidof -s {{package}})`

- Color the log (usually use with filters):

`adb logcat -v color`
