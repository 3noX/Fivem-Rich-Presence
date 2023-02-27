# Fivem-Simple-Discord-Rich-Presence
A simple fivem rich present with imgs and buttons. 😋

## Instructions Guide 🥰
### Step 1 🥀
Download () and copy [Discord](discord) Folder Into resources folder in your FiveM Server and Edit the `client.lua` file and don't edit `fxmanifest.lua` file.


### Step 2 🥀
Edit thing you should edit that comment said to
**Make sure to read all the comments**
**Get your Own Application from https://discordapp.com/developers/applications/**

**Example :**
```Citizen.CreateThread(function()
    while true do
        local player = GetPlayerPed(-1)
        
        Citizen.Wait(5*1000) -- checks every 5 sec.
        
        SetDiscordAppId() -- your application client id

        SetRichPresence( GetPlayerName(source) .. " is on " .. GetStreetNameFromHashKey(GetStreetNameAtCoord(table.unpack(GetEntityCoords(player))) )) -- main text

        SetDiscordRichPresenceAsset("") -- your large logo name here (.png, .jpg, or .jpeg — 1024x1024 recommended, 512x512 minimum)
        SetDiscordRichPresenceAssetText(GetPlayerName(source)) -- large logo hover text

        SetDiscordRichPresenceAssetSmall("") -- your small logo key
        SetDiscordRichPresenceAssetSmallText("Health: "..(GetEntityHealth(player)-100)) -- your small logo hover text (.png, .jpg, or .jpeg — 1024x1024 recommended, 512x512 minimum)

        SetDiscordRichPresenceAction(0, "Button 1", "https://discord.gg/kJu8ZPqTNF") -- Button 1 name and link
	    SetDiscordRichPresenceAction(1, "Button 2", "https://denuwanhackzzz.me") --  Button 2 name and link


    end
end)

--Barbie-Devs```
