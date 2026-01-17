---
title: "What happens if your hard drive dies tomorrow? My new 3-2-1 backup strategy."
summary: "Introduction to my new DAS setup and storage backup system."
description: "How I went from scattered photos and cloud-only storage to a reliable 3-2-1 backup strategy using a centralized DAS setup."
categories: [Homelab]
tags: [Homelab, DAS, NAS, Backup]
date: 2026-01-17
draft: false
---

{{< lead >}}
*«We do not remember days, we remember moments.»* — Cesare Pavese
{{< /lead >}}

You know that feeling when you tell yourself *“I don’t need that”* for months and then one night, usually way too late, you suddenly find yourself clicking *“buy now”*?

That was me with storage.

For a long time, I convinced myself that cloud storage was enough. Google Photos, iCloud, whatever — it’ll be fine, right? But then life happened. I started traveling more. My girlfriend and I both take photos. We have two phones, two desktops. I also spent weeks digitizing old photos from past trips.

And suddenly everything was… everywhere.

No real backup strategy. No clear source of truth. Just scattered copies and a thin layer of hope that nothing would fail.

This is how I fixed it — and why I ended up choosing a DAS (Direct Attached Storage) instead of the NAS everyone keeps recommending.

## The Problem Was Very Real

Picture this:
* Travel photos on my phone
* More photos on her phone
* Edited versions on one desktop… or maybe the other one
* Old digitized photos on an external drive somewhere (I think)

You get the idea.

We had photos spread across at least four devices, plus a couple of old hard drives. There was no central place. No proper backup. And the most worrying part? Those old digitized trip photos — the ones I spent hours scanning — existed in exactly one copy, on a hard drive that was already five years old.

That’s not a backup. That’s a countdown.

I needed something simple. Something reliable. Something that wouldn’t die and take our memories with it.

## Why I Chose a DAS Instead of a NAS

If you search online for storage advice, you’ll quickly hear: “Just get a NAS.” And honestly, I understand why. Network Attached Storage is powerful. Remote access, apps, media servers, users, permissions — the whole package.

But here’s the thing: I didn’t need all that.

At least, not yet.

A DAS is much simpler:
* You connect it directly to your computer via USB-C or Thunderbolt
* No network configuration
* No separate operating system
* No services running 24/7

It’s fast, straightforward, and predictable.

It’s also cheaper. A NAS with similar capacity and flexibility would have cost significantly more. The TerraMaster D8 Hybrid gave me eight drive bays without forcing me into a full server-style setup.

There’s also power consumption. A DAS only spins up when I’m using it. My electricity bill appreciates that.

And remote access? I don’t really need it right now. When I’m traveling, I’m taking photos — not browsing my archive. Maybe that changes in the future. But for now, direct attachment does exactly what I want.

## Designing a Real Backup Strategy (3-2-1)

Once I decided to centralize storage, the next step was more important than the hardware itself: backup strategy.

That’s where the 3-2-1 rule comes in:
* 3 copies of your data
* 2 different types of storage
* 1 copy off-site

Simple on paper, but incredibly effective.

And one crucial thing I learned early: RAID is not a backup. RAID protects you from a single drive failure. It does not protect you from accidental deletion, corrupted files, ransomware, or disasters like fire or theft.

So RAID helps — but it’s only part of the solution.

## My 3-2-1 Setup

### Primary storage: TerraMaster D8 Hybrid

This is where everything lives.

I configured the TerraMaster with RAID 5, which means I can lose one drive without losing data. Again, not a backup — but good protection against a disk dying unexpectedly.

I currently run four 4 TB drives, which gives me plenty of space for photos now, and room to expand later. Eight bays means I don’t have to rethink the whole setup every time storage grows.

Connected via USB-C, performance is more than good enough. I can browse, edit, and manage photos directly from the DAS without noticeable slowdown.

This is my source of truth.

### Secondary backup: Local external drive

The second copy lives on a completely separate external hard drive.

Once a week, automatically, the entire TerraMaster is backed up to this drive. Different hardware. Different connection. Stored in a different place in the apartment.

This protects me against:

* accidental deletions
* file corruption
* RAID failures
* “oops, I messed something up last week”

If something goes wrong, I can roll back.

### Off-site backup: Cloud (for the important stuff)

For the third copy, I use Backblaze.

Not everything goes to the cloud. Uploading every random RAW file would be expensive and unnecessary. But the important things do:

* final edited photos
* old digitized pictures
* irreplaceable memories

Backblaze runs quietly in the background and uploads when it can. Initial uploads take time, but that’s fine. This copy exists for worst-case scenarios: fire, theft, flood — anything that destroys everything local.