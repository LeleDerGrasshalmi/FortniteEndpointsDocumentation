# terminalCommandResult

**Description**: `A Terminal Command was Executed` \
**Operations**: [ExecuteTerminalCommand](../Operations/ExecuteTerminalCommand.md)

## Body

```js
{
    // standard profile notification content
    "type": "terminalCommandResult",
    "primary": true,
    "client_request_id": "",

    //specific to this notification
    "canRepeat": false,
    "rewardGranted": true,
    "successActionTag": ""
}
```
