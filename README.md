# Kevin M AMS2 Tower

Hi! This is a racing scoreboard for your game.

It floats on top of Automobilista 2 (AMS2). It shows who is in first place, who is in second, who is chasing you, and how far apart everyone is. It is called a "tower" because it is a tall list, like a tower of drivers.

You do not have to touch anything while you race. It changes by itself.

---

## What you need first

You need four things. Think of them like the ingredients for a sandwich.

1. **SimHub.** This is the free program that makes the tower appear. Version 9.11.22 or newer is best.
2. **Automobilista 2.** The tower only understands this game.
3. **The Gary Swallow plugin for SimHub.** This is a little helper that tells the tower the names and laps of every driver. **Without it, the tower will not work.** It is made by Gary Swallow, and it is free. You get it here:
   https://www.overtake.gg/downloads/simhub-tv-style-side-scrolling-leaderboards-timings-sidescreen.18746/
   You need a free OverTake.gg account to download anything from that site, so register there first. When you download it, **put in all of it, not just the one file that ends in .dll**. How to do that is explained below.
4. **A game setting.** In AMS2, go to Options, then System, then Shared Memory. Set it to **Project CARS 2**. Then close the game and open it again. (The game only reads this setting when it starts.)

---

## How to put it in

There are two steps. The first one is the plugin. The second one is the tower.

**Step 1: put in the Gary Swallow plugin**

1. Download the plugin from the link above. It comes as a zip file.
2. Unzip it, and **keep everything that is inside**. The plugin is not just one file. There is a file that ends in **.dll**, and there are folders that belong with it. The plugin needs those folders to do its job.
3. Close SimHub.
4. Copy **everything** from the zip into the main SimHub folder. Usually that is here:
   `C:\Program Files (x86)\SimHub`
   If Windows asks whether you want to join or replace folders, say yes.
5. Right click the .dll, choose Properties, tick **Unblock** if you see it, and press OK. (Windows sometimes locks files that came from the internet.)
6. Open SimHub. Go to Settings, then Plugins, and switch the Gary Swallow plugin **on**. Restart SimHub if it asks.

> **Please do not copy only the .dll file.**
>
> This is the easiest mistake to make, and it is a sneaky one, because nothing looks broken. SimHub opens. The plugin looks switched on. The tower even shows up on your screen. But the list of drivers stays empty, for ever, and nothing tells you why.
>
> Here is what happens. The plugin wants to write into a folder called **RaceResults**. That folder comes in the zip. If you copied only the .dll, the folder is not there, so every time the plugin tries to write, it trips over and stops. It never gets as far as telling the tower who the drivers are.
>
> Copy the whole zip and this will not happen to you.

**Step 2: put in the tower**

1. Unzip the download. Inside is a file called **Kevin M AMS2 Tower.simhubdash**. Double click it. SimHub puts the tower in for you.
2. In SimHub, find **Kevin M AMS2 Tower** in your dashboards and turn it on as an overlay.

The tower is tall and skinny (650 wide and 1440 tall). Put it at the side of your screen.

---

## What you will see

The tower is a list of drivers. Each driver gets a row with their position and name, like "L. HAMILTON". **You are the gold row**, so you can always find yourself.

### In practice and qualifying

* Everyone's best lap time.
* Three little boxes for each driver, one for each part of the track. The colour tells you how good that part of the lap was.
* A "!" mark if a lap does not count.
* "OUT LAP" when a driver has just left the pits.
* A "winner" banner when the time runs out.

### In the race

* The order of the drivers.
* How far each driver is behind. The numbers switch back and forth between "how far behind the leader" and "how far behind the car in front".
* A blue **P** when a driver is in the pit lane.
* A green or red number showing how many places a driver has gained or lost since the start.
* A little badge for the driver with the fastest lap.
* A "+1 LAP" tag for a driver who has stopped and fallen a lap behind.
* "LAST LAP" and "FINISH" near the end of timed races.
* A checkered flag and a winner banner when the race is over. After that, each driver shows how many pit stops they made.
* A little "+5s" tag if **you** get a time penalty. (The game does not give penalties to computer drivers, so the tower only watches you.)

### The top bar

* The track name and the time left.
* Your position and your lap.
* The weather: sun, clouds, rain, and the air and track temperature.
* Flags: yellow, blue, black, green, white, red and more.
* A warning when rain is coming.

### The bottom box

* How much fuel you have left.
* Your current lap time and your last lap time.
* How much faster or slower you are than before.

---

## The different towers

There are several towers in the one package. Pick the one you like best.

* **Large Race Tower.** Lots of rows. Good for big races.
* **Small Race Tower.** A shorter list.
* **Large Race Tower Team Image.** Same as the large one, but each driver gets a little car maker picture.
* **Multi Class Tower.** For races with different kinds of cars. It sorts the drivers into groups, and shows you and the drivers near you.
* **Full Field Tower.** Shows the whole field in one long list.
* **Practice and Qualify towers.** Large, small and multi class versions.
* **Time Trial Tower.** For time attack.
* **Garage.** Shows up while you are in the garage.

The tower picks the right group by itself. It knows if you are practising, qualifying or racing. If you want a different one inside the same group, use SimHub's screen switching. You can give it a button or a key.

The tower has to be small enough to fit on your screen, so it cannot show every single driver at once. When there are lots of cars, it shows the drivers at the front and the drivers near you.

---

## If something looks wrong

**The tower is empty, or the names are missing.**
Check these four things, in this order. The first one is the most common by far.

1. **Did you copy the whole Gary Swallow download, and not just the .dll?** Open this folder:
   `C:\Program Files (x86)\SimHub\DashTemplates\GS - Options`
   Look for a folder inside it called **RaceResults**. If it is not there, that is your problem. Go back to Step 1 and copy everything from the zip. If you would rather fix it by hand, you can simply make a new empty folder there and call it `RaceResults`.
2. **Check the game setting.** In AMS2: Options, then System, then Shared Memory, set to **Project CARS 2**. Then close the game and open it again. The game only reads this when it starts.
3. **Check the plugin is on.** In SimHub: Settings, then Plugins, and make sure the Gary Swallow plugin is switched on.
4. **Check Windows is not blocking it.** If you cannot see the plugin in that list at all, right click the .dll file, choose Properties, tick Unblock, and restart SimHub.

If it still will not work, you can peek at SimHub's diary. Open this file in Notepad:
`C:\Program Files (x86)\SimHub\Logs\SimHub.txt`
Search it for the word **ERROR**. If you see a line about `RaceResults`, it is problem number 1 above.

**There are thin lines between the rows.**
Windows might be making things bigger. Go to Windows Settings, then Accessibility, then Text size, and set it back to 100%.

**The words look strange.**
The tower comes with its fonts, and SimHub puts them in for you when it installs the tower. Close SimHub and open it again. If the words still look strange, the fonts are also in a folder called **_SHFonts**, inside the tower's folder in SimHub's DashTemplates folder. Select all the fonts there, right click, and choose Install.

**The tower disappears sometimes.**
That is on purpose. It hides while you wait for a race to start, and when your race is over and you are back in the pits.

---

## Good to know

* It was made for Automobilista 2 and tested there. It may not work in other games.
* The gaps between drivers are good estimates, not perfect measurements.
* The tower uses the Gary Swallow plugin for its driver information. That plugin belongs to Gary Swallow, and it is not part of this download. Thank you, Gary!
* It was made by Kevin M. Have fun, and race safe!
