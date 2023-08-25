# Progressbar
Just a small, simple release for the QBCore Community. In anticipation of a series of releases we have planned over the coming weeks we have dropped this small html edit on the qbcore dependency 'progressbar' for the community. This is our second release for this with a different design, We hope you like it.  

Preview (Imgur): 

https://i.imgur.com/but68PA.png

https://i.imgur.com/E92tE4l.png

https://i.imgur.com/hbF066V.png

Any questions, join our discord community at: https://discord.gg/fTGm36CERk


# Usage

## QB-Core Functions

### Client

- QBCore.Functions.Progressbar(**name**: string, **label**: string, **duration**: number, **useWhileDead**: boolean, **canCancel**: boolean, **disableControls**: table, **animation**: table, **prop**: table, **propTwo**: table, **onFinish**: function, **onCancel**: function)
  > Create a new progressbar from the built in qb-core functions.<br>
  > **Example:**
  > ```lua
  >QBCore.Functions.Progressbar("random_task", "Doing something", 5000, false, true, {
  >    disableMovement = false,
  >    disableCarMovement = false,
  >    disableMouse = false,
  >    disableCombat = true,
  >}, {
  >    animDict = "mp_suicide",
  >    anim = "pill",
  >    flags = 49,
  >}, {}, {}, function() -- Done
  >    StopAnimTask(PlayerPedId(), "mp_suicide", "pill", 1.0)
  >end, function() -- Cancel
  >    StopAnimTask(PlayerPedId(), "mp_suicide", "pill", 1.0)
  >end)
  > ```
