---
layout: default
title: Server Management
parent: Playing Online
nav_order: 3
published: true
---
## Server Management

![Server manager.png]({{site.baseurl}}/Images/Online/Server manager.png)

Once you reach the point where one server isn't enough, you can start using a Server Manager. It's a simple program that let you manage server and redirect clients and it works with both game servers and communication servers. Each Server Manager can only have either game servers or communications servers as it can't identify what it's managing.

Instead of having players connect to a game/communication server, they will connect connect to the Server Manager which will redirect them to the server that's the most appropriate. Usually that mean sending them to a populated server that's not full.

The Sever Manager work by manually adding existing servers to it, then it can keep track of them and put them to idle if there's more servers than players. If there's a spike of population it will use those servers first instead of trying to create new ones.


![Master.png]({{site.baseurl}}/Images/Online/Master.png)

If you want to go another step and want multiple Server Managers, you'll want to use Masters. Same principle as the Server Manager, they will redirect player to Server Managers based on how populated they are.
Each master contains the list of every other master and every Server Manager so they can check the health of the infrastructure and act as a fallback point if a Server Manager or a Game/Communication server die.