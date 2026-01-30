## MR-Plus [![Build Status](https://github.com/Hexeption/MCP-Reborn/workflows/Java%20CI/badge.svg)](https://github.com/Hexeption/MCP-Reborn/actions?workflow=Java+CI)

**Developer:** Treaki  
**Status:** Public Beta Source  
**Framework:** MCP-Reborn  
**Platform:** Minecraft Java Edition (PC)

---

## Overview

Minecraft Revival+ is a custom Minecraft client modification project focused on enhancing the base game experience through interface improvements, multiplayer upgrades, performance optimization, and experimental features.

This repository contains the public beta source release intended for developers, testers, and contributors who want early access to the project and its systems.

This is not a final build. Features may change or be removed as development progresses.

---

## Project Goals

The main objectives of this project include:

- Improving menu and interface usability  
- Enhancing multiplayer systems  
- Adding quality-of-life features  
- Optimizing client performance  
- Creating a flexible foundation for future development  

---

## Core Features

### Custom Multiplayer System

The multiplayer interface has been extended to support:

- Built-in server injection logic  
- Improved server selection handling  
- Custom button integration  
- Server protection rules  
- Enhanced connection flow  

Important related files include:

- `MultiplayerScreen.java`  
- `ServerSelectionList.java`  
- `ServerData.java`  

---

### Username Override System

A custom username input system has been implemented that allows:

- Manual username editing  
- Persistent username saving  
- Runtime session modification  

This system is handled through custom UI screens and session override logic.

Related logic can be found in:

- `UsernameScreen.java`  
- `Session.java` modification handlers  

---

### UI & Menu Improvements

Several UI components have been modified to improve usability and appearance, including:

- Button layout improvements  
- Navigation flow changes  
- Custom screen transitions  
- Additional menu actions  

These modifications mainly affect:

- `Screen.java` based classes  
- Custom GUI screens  
- Button interaction handlers  

---

### Performance Optimizations

Early-stage performance improvements focus on:

- Reducing unnecessary UI refresh calls  
- Improving render efficiency  
- Cleaning redundant processing logic  
- Optimizing server list refresh behavior  

---

## Build Requirements

To compile this project you will need:

- Java JDK 8 – 17  
- Gradle  
- MCP-Reborn environment  
- An IDE such as IntelliJ IDEA or Visual Studio Code  

---

## Build Instructions

Clone the repository:

`git clone https://github.com/treakiii/MinecraftRealistic-.git`

Wait for gradle things to install then click in the gradle right tab 
go to /Tasks then /mcp and then use the setup , then the copy assets and finally the run client.

`by Treaki , I hope that u like it`
