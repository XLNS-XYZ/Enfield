# Development Project Outline
This document should not be shared and should be kept confidencial.

This project outlines the basis of what the objectives and issues that the development process of Hackney may encounter. It is important to address these issues in a provocative manner so that **appropriate** forms of assets are created, preventing the waste of time.

Places
---
During the Hackney development, Three seperate places will be created:

* **Hackney Public Release Server**
* **Hackney Alpha Testing Server**
* **Hackney Asset Testing Server**

It is important to not directly edit in the Public Release server. Changes to the game should be made on the Alpha server and **satisfied**, be published towards the Public Release Server.

Hackney Asset Testing Server will be made for checking external assets, this documentation will cover that process.

Error Free Environment
---
In order to save time during the development process, Hackney may use previous assets of previous games. Each individual asset must be tested for the following:

* Internal Errors (Script Errors, Efficacy),
* Appropriate Part Count,
* FE Compatability.

If the asset fails to meet these standards, it will be fixed appropriately. Avoid adding assets which are difficult to fix. 

**DO NOT EVER ADD MODELS DIRECTLY INTO THE ALPHA SERVER EVEN IF IT IS TRUSTED AND ERROR FREE**

Game Limitations
---
Most of these limitations are aimed towards fighting lag, especially due to the game being FilteringEnabled. Understand the difference between **Client** and **Server** Lag:

Client Lag are mostly caused by excessive thread opening on the client side of users. Such as having too many scripts, parts and instances inside a client. It is highly suggested that localscripts should be kept to a minimum. External assets should be combined into one localscript. To combat these issues:

* Limit the number of scripts running on a Client.

Server Lag is mostly caused by numeric factors such as high part count, excessive textures, moving parts, physical properties. To combat these issues:

* Limit the number of parts in the game : 100k should be the maximum point.
* Try to keep parts thin if possible, reduce the size of the part, exceptions can be made for physics heavy objects such as roads.
* Reduce the need of Transparency and internal rendering: Glass effects, Transparency.
* Anchor parts which do not need to move.
* Union efficiently, Union if the part difference is high (i.e. 10 parts into 1), do not union 2 parts into 1.
* Put unreachable parts non collideable, so that the physics engine is leniant towards the parts.

Development Standards
---
If there is an issue with something being developed, it needs to be addressed immediatally. Do not be afraid to critisise someone's work. Because as soon as the result product of whatever they work on is finished, chances are deleting the asset would be unethical and a waste of time.

**We do not use free models**

Do not distrubute any assets or make it public unless permission is given. Risk mitigation of the game getting leaked should not be considered, this is applicable in the process of where developers are found.

#### Task Management

It is highly reccomended to not mix tasks within developers in terms of catagory; i.e. One person focuses on road creation, and one person focuses on exterior building creation.

Mixing these tasks can cause a large inconsistancy.

---

Project Manager - XLNS_XYZ
