---
layout: post
title: "Starting my Homelab"
date: 2026-09-02
author: "James"
---

## What is a homelab?

There isn't really a concrete definition. 

Put simply, it can be whatever you want it to be.

I've generally understood it as a personal environment to learn and experiment with technology. What you want to do and what kind of budget you have will very much affect what it is, but these constraints are usually what end up driving the learning process.

In my case, the goal was to gain more experience in infrastructure and networking to understand the underlying backbone that supports all modern systems. I wanted to learn how to build, break and hopefully fix things as I've found it's how I learn best. 

Fortunately, getting started doesn't require a huge budget. There's an abundance of used enterprise hardware that is cheap, compact and capable - more than capable of running the virtual machines I wanted to experiment with. 

This sounded like a sensible place to get started.

## Getting started

After talking to my manager, he suggested looking at mini PCs. He conveniently had two Dell Optiplex 7040 Micros he was looking to get rid of. 

At a great price and more than reasonable specs, I took both.

Having two identical machines gave me more than enough to start experimenting and meant I wasn't limited to running everything on a single host. The plan was to install Proxmox and use them to explore virtualisation across multiple machines, giving me room to learn about clustering, redundancy, failover and recovery.

For what I wanted to do, this was already more than enough - and with the addition of a cheap switch to connect them, I could've stopped there.

## My horrible spending habit

I did not stop there.

Once I started looking through used hardware, it became too easy to justify adding to the lab. A few good eBay deals later, I had already added an Optiplex 7060 Micro and 7060 SFF within the space of a week.

Then came the networking. I picked up a Unifi 8-port 2.5GbE PoE switch, giving me a managed switch and capability to accomodate PoE (Power over Ethernet) devices to my setup. This was followed by a Unifi U6 Pro access point, and eventually a Lenovo ThinkCentre M720q which I planned to turn into a dedicated router with a PCIE riser and four-port Intel I350 NIC.

I had suddenly ended up with a leaning tower of hardware on my desk, having set up absolutely nothing on the hardware I started with.

## "Futureproofing"

Most of these purchases fell under the perfectly reasonable justification that I was "futureproofing".

This is the most dangerous word to learn when dealing with hardware.

Spending more to save money in the long run is usually the smart choice, but it's extremely easy for it to become an excuse to spend more on things you simply dont need. I didn't _need_ 2.5GbE networking, and most of my devices currently support up to 1GbE, but I might _eventually_.

While these decisions made sense individually, I was left with much more hardware than I had any immediate use for. Despite approaching this stage the wrong way, having more resources than necessary gave me a lot of headroom to experiment and run heavier loads on my servers.

I now have to find things to run on all of my hardware instead of buying hardware for things I want to run. Ironically, this motivates me to do more with my homelab to make sure it doesn't end up being a waste of money.

## Final inventory

|---|---|
| **2x Dell OptiPlex 7040 Micro** | i7-6700T · 64 GB RAM · 256 GB SATA + 256 GB NVMe SSD |
| **Dell OptiPlex 7060 Micro** | i7-8700T · 32 GB RAM · 256 GB SATA SSD |
| **Dell OptiPlex 7060 SFF** | i7-8700 · 32 GB RAM · 512 GB SATA SSD |
| **Lenovo ThinkCentre M720q** | i5-8500T · 8 GB RAM · 256 GB NVMe SSD |
| **UniFi USW-Flex-2.5G-8-PoE** | 8-port 2.5GbE · PoE |
| **UniFi U6 Pro** | Wi-Fi 6 · PoE access point |

It's far more than I need to get started, but now I have plenty of room to experiment with almost anything I can think of.

The next step is to put it to use, starting with the network everything else will depend on.