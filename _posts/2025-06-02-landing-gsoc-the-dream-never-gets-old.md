---
layout: post
title: 'Landing GSoC: The Dream Never Gets Old'
date: 2025-06-02 19:20 +0530
---

I'm excited to announce that I've been selected for **Google Summer of Code 2025**, where I’ll be working with the **KDE Community** to create a **mobile application for Mankala** using **Qt and QML**.

This project is a continuation of my earlier work during *Season of KDE*, where I integrated the **Pallanguli** variant into the MankalaEngine. With the core engine now supporting multiple game variants, my focus for this summer is to design a mobile interface that makes playing Mankala more accessible and enjoyable on handheld devices.

## Project Goals

The primary objectives of my GSoC project are:

- Design and implement a mobile-friendly UI using **Qt Quick/QML**
- Add support for **multiplayer gameplay**, enabling users to connect and play in real-time
- Integrate **XMPP protocol** for communication, leveraging KDE’s existing ecosystem where possible

The multiplayer component is particularly important to me. Mankala is traditionally a social game, and enabling real-time remote play will bring the experience closer to its roots. XMPP is a strong candidate for this feature due to its extensibility and compatibility with open-source principles.

## Building on Previous Work

During **Season of KDE**, I worked on researching and integrating **Pallanguli**, a traditional South Indian variant, into the **MankalaEngine**. This involved implementing its unique gameplay mechanics, refining move and turn logic, and ensuring smooth integration with the existing game engine. I also developed a **Terminal User Interface (TUI)** for Pallanguli, enabling quick testing and easier interaction in headless environments.

Beyond my own contributions, the Season of KDE cohort worked collaboratively to enhance MankalaEngine significantly:

- **Shubham** implemented Monte Carlo Tree Search and a Reinforcement Learning agent for smarter AI, along with writing unit tests using QTest.  
- **Ashutosh** developed a desktop GUI for MankalaEngine using QML and Kirigami, improving the overall user experience.  
- **Rishab** integrated the popular Kalah variant, expanding the game’s variety.  
- **Nidhish** added PvP functionality using the XMPP protocol, laying the foundation for multiplayer gameplay.  

Currently, board synchronization during multiplayer is done manually; I plan to automate and enhance this as part of my GSoC work.

I also submitted a **Bugzilla request** to package the application for **Fedora Linux**, contributing to its availability on Linux distributions.

Beyond development, I conducted an **Open Source Meetup** at my college, introducing students to KDE applications and encouraging hands-on contributions to free and open-source software.

Now, I’m looking forward to taking on a more user-facing challenge, where **UI/UX, networking, and performance** all come together.

## Community Bonding Phase

During the Community Bonding period, I took the opportunity to strengthen my understanding of the tools and technologies that will drive this project. I focused on:

- The **Qt framework**, including its architecture and modular structure
- **QML and Qt Quick**, for building responsive and modern UIs
- **QWidgets**, to understand the differences between traditional desktop and declarative UI development
- **Network programming with Qt**, as preparation for integrating multiplayer functionality and XMPP-based communication
- I tried creating artworks using **Krita**, but they look far from post worthy.

These learnings have helped me prepare a more concrete development plan and will guide my implementation choices throughout the summer.

## Detailed Project Timeline

### June 2 – June 13  
**Task:** Implement the Core Game Board UI  
- Develop a responsive and reusable QML component for the Mankala board  
- Ensure it supports all existing Mankala variants (e.g., Pallanguli) through flexible bindings to the engine  
- Design with mobile-first principles, ensuring touch responsiveness and orientation adaptability  

### June 16 – June 27  
**Task:** Build Navigation and Local Multiplayer  
- Create supporting UI pages:  
  - Welcome screen  
  - Menu/Variant selection  
  - Game over/Score display  
- Implement **Pass-and-Play** mode for local PvP  
- Add support for navigation and basic user interaction flow  

### June 30 – July 11  
**Task:** Integrate AI and Midterm Preparation  
- Integrate the existing `MankalaEngine` for **Player vs Computer (PvC)** mode  
- Add basic game difficulty configurations (if feasible)  
- Begin and finalize **developer documentation** using `QDoc`  
- Ensure project is ready for **midterm evaluation**

### July 21 – August 1  
**Task:** Start Multiplayer – XMPP Setup  
- Set up basic **XMPP client integration** using `QXmpp`
- Implement player presence and availability indicators  
- Begin work on peer discovery and invitation mechanisms  

### August 4 – August 15  
**Task:** Multiplayer Game Logic  
- Sync board state across devices using XMPP messaging  
- Handle move transmission, turn tracking, and error cases  
- Add reconnection logic and basic game state recovery (if possible)  

### August 18 – August 22  
**Task:** Finalize Multiplayer + Distribution  
- Refine multiplayer logic with edge case handling (e.g., mid-game quit, invalid moves)  
- Evaluate publishing options:  
  - **F-Droid** (via KDE’s infrastructure)  
  - **Google Play Store** (manual testing + metadata preparation)  
- Add privacy notice and handle basic app permissions (e.g., internet access)  

### August 25 – August 29  
**Task:** Final Week – Polish and Document  
- Bug fixing and performance tuning  
- Finalize user and developer documentation  
- Tag release candidate and ensure build reproducibility  
- Submit final blog post and project report  

## Next Steps

With the bonding phase complete, I’m now moving into the initial development stages. My immediate goals include:

- Setting up the base project structure  
- Implementing the core UI for the game board using QML   

I’ll be sharing regular progress updates through KDE channels and my blog, reflecting on both technical milestones and the broader experience of working on an open-source mobile game.

I’m grateful to **KDE**, **my mentor Benson Muite**, and **Google** for this opportunity. I look forward to contributing something meaningful to the KDE ecosystem while continuing to grow as a developer.

This summer marks the beginning of another exciting chapter in my journey with open source.

