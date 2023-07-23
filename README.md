# fluidMobile
Quick and easy way to add mobile compatibility; not advised for extensive button usage.

Simple example:
```lua
local onMobile = fluidMobile:isMobile()
if onMobile then
  fluidMobile.Initialize() -- must do this
  --
  local newButton = fluidMobile.newButton{
    Image = 'randomImageIdHere',
    Text = 'hi' -- note that only one will work. either you put text, or an image; you cannot do both.
  }
  newButton.Held:Connect(func1)
  newButton.Released:Connect(func2)
  newButton:Destroy()
end
```
