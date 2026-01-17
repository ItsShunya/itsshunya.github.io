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

You know that feeling when you tell yourself *“I don’t need that”* for months, maybe years — and then one night you suddenly click *“buy now”*?

That was me with storage.

For a long time, I convinced myself that cloud storage was enough. Google Photos, iCloud — it'll be fine. Then I started traveling more. My girlfriend and I both take photos, lots of them, and everytime we returned from a trip we had a thousand more photos.

And suddenly everything was everywhere.

No clear structure. No real backup strategy. Spending a lot on cloud storage, local copies scatter on our phones and the hope that nothing would fail.

This is how I fixed it — and why I ended up choosing a DAS (Direct Attached Storage) instead of the NAS everyone seems to recommend.

## The Problem: Photos Everywhere, Backups Nowhere

Photos lived on phones, desktops, old external drives. Edited versions here, originals there. Some files existed in multiple copies, others in exactly one. The worst part? The old digitized travel photos — hours of work — were stored on a single aging hard drive.

That’s not a backup. That’s a risk.

I needed a single place for everything, plus real backups.

## Why I Chose a DAS Instead of a NAS

If you read forums, the answer is always: “Get a NAS.” And sure, NAS devices are powerful. Remote access, apps, services, media servers.

But I didn’t need a server. I needed storage.

A DAS is simple:
* direct USB-C connection
* no network configuration
* no always-on system
* lower cost and power usage

The TerraMaster D8 Hybrid gave me eight drive bays, good performance, and room to grow — without the complexity or price of a full NAS. It connects directly to my computer and just works.

Remote access can come later. For now, simplicity wins.

## My 3-2-1 Backup Setup

Once I decided to centralize storage, the next step was more important than the hardware itself: backup strategy.

That’s where the 3-2-1 rule comes in:
* 3 copies of your data
* 2 different types of storage
* 1 copy off-site

### Primary storage

This is where everything lives.

I configured the TerraMaster with RAID 5, which means I can lose one drive without losing data. Again, not a backup — but good protection against a disk dying unexpectedly.

I currently run four 4 TB drives, which gives me plenty of space for photos now, and room to expand later. Eight bays means I don’t have to rethink the whole setup every time storage grows.

Connected via USB-C, performance is more than good enough. I can browse, edit, and manage photos directly from the DAS without noticeable slowdown. This is my source of truth.

### Secondary backup

The second copy lives on a completely separate external hard drive.

Once a week, automatically, the entire TerraMaster is backed up to this drive. Different hardware. Different connection. Stored in a different place in the apartment.

This protects me against accidental deletions, file corruption, RAID failures and the typical “oops, I messed something up last week”. If something goes wrong, I can always roll back.

### Off-site backup

Not everything goes to the cloud. Uploading every random RAW file would be expensive and unnecessary. But the important things do:

* Personal documents.
* Photos I don't want to lose.

## Lessons Learned (And Was It Worth It?)

The TerraMaster D8 Hybrid wasn’t cheap, but compared to the value of photos I can’t replace, it was absolutely worth it.

If you’re telling yourself “I don’t need that”, ask one question:

What happens if your current storage dies tomorrow?

If that makes you uncomfortable, you already have your answer.

I know — because I was you not long ago.