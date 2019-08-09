# ClashRoyale (2017)
[![clash royale](https://img.shields.io/badge/Clash%20Royale-1.9.2-brightred.svg?style=flat")](https://clash-royale.en.uptodown.com/android/download/1632865)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Build status](https://ci.appveyor.com/api/projects/status/dmt9bk3bf1kaxnoa?svg=true)](https://ci.appveyor.com/project/Incr3dible/clashroyale)

#### A .NET Core Clash Royale Server (v1.9)
##### If you want to test the current build you can download [this](https://retroroyale.xyz) client.

## Battles
The server supports battles, for those a patched client is neccessary.

[See the wiki for a tutorial](https://github.com/retroroyale/ClashRoyale/wiki/Patch-for-battles)

## How to start

#### Requirements:
  - [.NET Core SDK 2.2.x](https://dotnet.microsoft.com/download/dotnet-core/2.2)
  - Redis server
  - MySql Database (on Ubuntu i suggest WAMP with PhpMyAdmin)

for Ubuntu use these commands to set it up:
```
git clone https://github.com/retroroyale/ClashRoyale.git && cd ClashRoyale/src/ClashRoyale

dotnet publish "ClashRoyale.csproj" -c Release -o app
```
To configurate your server, such as the database you have to edit the ```config.json``` file.

#### Run the server:

```dotnet app/ClashRoyale.dll```

#### Update the server:

```git pull && dotnet publish "ClashRoyale.csproj" -c Release -o app && dotnet app/ClashRoyale.dll```

## Need help?
Contact me on Discord (Incredible#2109) or open an issue.
