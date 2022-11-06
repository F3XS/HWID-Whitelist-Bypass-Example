Yes it's simple here is example

```
local mag; mag = hookfunction(game.HttpGet, function(self, url, ...)
    if url:find("aimstudio") then
        local old = url:split("user=")
        local new = old[1] .. "1" .. "&hwid=" .. "8cd08b2a05e9fd58352edaa5f1215162861211cf53054191d9fbb761b043391d9348a0541d01e7f66aab52291768d2ad07489fa3073a279cad360540a1681e76"
        return mag(self, new, ...)
    end
    return mag(self, url, ...)
end)

loadstring(game:HttpGet("https://raw.githubusercontent.com/F3XS/HWID-Whitelist-Bypass-Example/main/The%20Script%20I%20am%20about%20to%20Bypass"))()```
