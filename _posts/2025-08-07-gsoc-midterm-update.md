---
layout: post
title: GSoC Midterm Update
date: 2025-08-07 12:53 +0530
---

We’re already halfway through GSoC 2025, and it’s been a really exciting journey so far working with the Mankala Engine under KDE. Here’s a quick update on what I’ve been up to and what’s coming next.

### Core Game Board UI

The first big task was building the core Mankala board using QML. The goal was to make it reusable, responsive, and able to support different game variants like Pallanguli. That’s now done!

The board adapts based on screen size, so whether you're on a phone or desktop, in landscape or portrait mode, it just works. Touch interactions are smooth too, which is especially important for mobile users.

Here’s how the game board looks:

**Landscape Mode:**

![Landscape Game Board](/assets/Landscape-GameWindow.jpeg)

**Portrait Mode:**

![Portrait Game Board](/assets/Portrait-GameWindow.png)

### Navigation and Local Multiplayer

Once the board was ready, I focused on creating the rest of the UI. So far, I’ve built:

- A Home Screen

![HomeScreen](/assets/HomeScreen.png)

- A Rules page

![RulesPage](/assets/RulesPage.png)

- A menu for selecting game variants
- The main game screen (in both portrait and landscape)
- A game over/score display screen

I also implemented a pass-and-play mode so two players can play locally on the same device. The overall navigation between these screens is working well and feels smooth.

### AI Integration and Midterm Prep

The next step was adding support for playing against the computer. That’s now complete using the existing MankalaEngine. You can now play solo against an AI opponent, and it handles moves correctly.

Right now, I’m working on writing developer documentation using QDoc. The goal is to make sure everything is clear and easy to understand for anyone who wants to contribute later on.

### What’s Done So Far

- Built the reusable QML game board
- Created responsive layouts for different orientations
- Implemented navigation and local multiplayer
- Integrated AI for single-player mode
- Documentation is in progress

I’m happy with the progress so far, and the project is in good shape for the midterm evaluation. In the next phase, I’ll be polishing the interface, finishing up the docs, and implement **Multiplayer Online play** using **XMPP**.

Also, just received my T-Shirt for contributing and successfully completing Season of KDE'25.

Thanks to my mentor **Benson Muite** and the **KDE community** for all the support so far. Looking forward to the next half of GSoC!

