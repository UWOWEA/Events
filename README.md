# Uwowea Events

`UwoweaEvents.EventName` is the event-name type for Blizzard frame events. It
aliases LuaLS's `FrameEvent` type from the WoW API annotations, so completion
uses the API's event list instead of maintaining a duplicate list here.

```lua
---@param event UwoweaEvents.EventName
local function Register(event)
    frame:RegisterEvent(event)
end
```

The available names follow the WoW API annotation version configured in
`.luarc.json`; the set can vary between WoW clients and API versions.
