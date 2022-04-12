---
layout: default
title: Server Startup
parent: Playing Online
nav_order: 1
published: true
---
## Server Startup

Let's start building up a server, it's pretty straight forward and you'll only need to play with the Connection Info.ini file.

The first thing you'll want to decide on is if you want to host your database or if you want to use MongoDB cloud database.
In the config file, look up to the **[Game Server Info]** tag. You can use **Connection Chain=Local** to use a local database or you can use **Connection Chain=mongodb+srv:[your connection information]**

Set the **Public Port** if needed, this is where the players will connect to play.
For the **Public IP** you can leave it as **127.0.0.1** if you plan on only having one server. It's only used to identify servers when transfering players between multiple servers. If you do have multiple server, use the public IP of the server.

You also need to look up **[User Information Info]** and set a **Connection Chain** for it as well. Odds are you'll want to use the same as above but you have the possibility to use a different database. However you can't have one Local and one being MongoDB.
