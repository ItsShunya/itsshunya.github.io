---
title: "'Hello World': A Small Start"
summary: "My first post on this new blog — where I'll start sharing notes, ideas, and things I learn along the way."
description: "Welcome to my blog. After finishing my website, this post is a small introduction to who I am, what I do, and what I plan to share here."
categories: [History]
tags: [Hello World, History]
date: 2025-11-29
draft: false
---

{{< lead >}}
*«The beginning is the most important part of the work.»* — Plato
{{< /lead >}}

A few days ago, while I was writing the introductory post for this blog — which I named “Hello World” (give it a read if you haven’t yet!) — I started thinking about this little tradition. I remembered reading something about its origin some time ago, so I thought it would be a good first post to dig into… or second, I guess? Either way, it felt like the right topic to start with.

{{< article link="/posts/20251128-intro/" showSummary=true compactSummary=true >}}

## What is "Hello World"?

When people begin learning programming, the very first program they usually write is called **“Hello World”**. It is a tiny piece of code whose only purpose is to show some text on the screen. Nothing fancy, nothing complex — just a simple confirmation that everything works: the compiler, the editor, the environment, and of course, the programmer.

A Hello World is like saying: *“Okay, I’m here. Let’s begin.”*

## What It Looks Like

In most high-level languages, printing text is extremely simple. For example, in *Python*:

```py
print("Hello, World!")
```

Or in *C*, which is a bit more verbose:

```c
#include <stdio.h>

int main(void) {
    printf("Hello, World!\n");
    return 0;
}
```

Even if these examples look trivial, they represent an important moment. They are the first successful interaction with a new language or toolchain.

## A Short History

The concept has a long history. One of the earliest known appearances is in **“*A Tutorial Introduction to the Language B*”** (1972), written by *Brian Kernighan*. In that tutorial, there is a small program that simply prints *“hello, world”*. This was probably the first time the phrase appeared in a programming example, the example in the book is shown below.

```b
main( ) {
        printf("hello, world");
}
```

{{< alert "search" >}}
The language *B* itself was a precursor to *C*. It was a simplified and typeless language developed at Bell Labs, mainly influenced by BCPL. It ran on the PDP-11 and other early systems, and it helped set the foundation for the more structured and powerful C language that would come shortly after.
{{< /alert >}}

A few years later, in 1978, *Kernighan* and *Ritchie* published the now classical book *“The C Programming Language”*, usually called *K&R*. This book contained a *Hello World* example very similar to the one we still use in *C* today. Because the book became extremely influential, the Hello World example became a standard tradition across the programming world.

Since then, almost every new language or tutorial starts with some variation of *“Hello, World!”*.

## Meet Blinky!

While Hello World works well for desktop or scripting languages, it does not make much sense in embedded development.

Most microcontrollers do not have:

- a screen
- a console
- a standard output
- or even an operating system

So… printing text is simply not an option.

In embedded systems, the equivalent of Hello World is known as **“Blinky”**: a tiny program that turns an LED on and off in a loop. Usually this LED is part of a development board. If it blinks, it means the firmware is running, the clock is configured correctly, the toolchain works, the programmer flashed the microcontroller successfully, and the device is alive.

A typical blinky in C might look like this (conceptually):

```c
int main(void) {
    setup_gpio_led();

    while (1) {
        toggle_led();
        delay_ms(500);
    }
}
```

This small blinking LED is the embedded developer’s version of printing “Hello, World!”. It is the first confirmation that the hardware, the toolchain, and the firmware setup are all correct.

## A Simple Beginning

Whether it’s a message on the screen or a blinking LED on a board, every project starts with a tiny signal: *"Hello, I’m running"*. It’s a small step, but it carries a lot of meaning. From this little beginning, entire systems and products eventually grow.

For me, writing this blog feels a bit like that first Hello World. A simple moment, but the start of something new.

More posts will come soon — and hopefully more interesting than blinking LEDs.