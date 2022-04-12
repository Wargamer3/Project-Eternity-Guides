---
layout: default
title: Communication Server
parent: Playing Online
nav_order: 2
published: true
---
## Communication Server

The communication server is essentially the same as the game server but isn't dependent on any game so it can even do cross game type communications. You'll only need to play with the Connection Info.ini file. It's optionnal and the game will work even without it so if you prefer to use third party applications to communicate you can skip this part.

The first thing you'll want to decide on is if you want to host your database or if you want to use MongoDB cloud database.
In the config file, look up to the **[Communication  Server Info]** tag. You can use **Connection Chain=Local** to use a local database or you can use **Connection Chain=mongodb+srv:[your connection information]**

Set the **Public Port** if needed, this is where the players will connect to play.
For the **Public IP** you can leave it as **127.0.0.1** if you plan on only having one server. It's only used to identify servers when transfering players between multiple servers. If you do have multiple server, use the public IP of the server.

You also need to look up **[User Information Info]** and set a **Connection Chain** for it as well. Odds are you'll want to use the same as above but you have the possibility to use a different database. However you can't have one Local and one being MongoDB.
