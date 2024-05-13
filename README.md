# Celery-supported-scripts
Without using Custom UNC script, here is a list of loadstrings celery can run by default.<br>
Unless your custom celery has the auto detect loadstring, then use the code below to run loadstrings, add it to the top before the loadstring <br>
```lua
--Credits to len
function httpget(url)
    local d,ise,Body=false,false,""
    game:GetService("HttpService"):RequestInternal({Url = url,Method = "GET"}):Start(function(suc, res) if not suc then Body = res.StatusCode ise = true d=true return end Body=res.Body d=true end)
    repeat task.wait() until d
    if ise then error(Body, 0) end return Body
end

function getgenv()
    return getfenv(2)
end

loadstring = getfenv().load_string
getgenv().loadstring = loadstring

if not getgenv().currGame then
    getgenv().currGame = game
end
local oldGame = getgenv().currGame
--Script orignally by 
local game = setmetatable({}, {
    __index = function(t,v)
        if v == "HttpGet" then
            return function(_,url)
                return httpget(url)
            end
        end
        if v == "GetService" then
            return function(_,a)
                return oldGame:GetService(a)
            end
        end
        if v == "FindService" then
            return function(_,a)
                return oldGame:FindService(a)
            end
        end
        return oldGame[v]
    end
})
```


**Scripts** <br>
Infinite yield <br>

```lua
loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
```
