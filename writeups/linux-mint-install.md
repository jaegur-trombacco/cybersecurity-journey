# Installing Linux Mint on a Used Build

## What I set out to do

I picked up a used custom build (ASRock Z77 motherboard, Intel i7-4790K,
GTX 1050 Ti) to learn hardware hands-on. The goal was to get a clean,
working OS on it — I landed on Linux Mint 22.3 Cinnamon. I chose Linux to 
start familiarizing myself with it for the cloud/security path since most 
cloud infrastructure and security tooling runs on Linux. 

## What went wrong / surprised me

The first wall I hit: the machine powered on, but I got no display at all —
no BIOS, no POST screen, nothing. My first assumption was the worst case: a
dead GPU or a bad motherboard.

After checking connections, I realized the problem. I'd plugged the monitor
into the motherboard's video output instead of the GTX 1050 Ti. With a
discrete graphics card installed, the onboard output was inactive — so the
screen stayed black even though the system was running fine. Moved the cable
to the GPU's port and the BIOS came right up.

It's a small fix, but it's a textbook "no display output" troubleshooting
scenario — and it maps directly to the A+ Core 1 objective on checking
onboard vs. discrete graphics when there's no video. Good reminder that the
obvious-in-hindsight cause is worth checking before assuming hardware failure.

## How I worked through it

Once I had display, the install itself was straightforward. I downloaded
the Linux Mint image and wrote it to a USB flash drive to make it bootable.

This was my first time actually doing this, but from studying I understood
that a machine will often try to boot from a plugged-in USB drive before the
internal drive. So I left the flash drive in at startup to test whether it
would catch — and it did. The machine booted into the Mint installer, and
from there I followed the guided installation to get Mint onto the internal
drive.

## Verifying the result

After install, I ran SMART health checks on the drive using smartmontools to
confirm the disk was healthy — worth doing on any used machine, since you
don't know how the previous owner treated the hardware. The overall health
assessment came back as passing, which was the main thing I wanted to
confirm before relying on the drive.

## What I'd do differently

Check the obvious physical connections before assuming a component failed.
Plugging into the GPU rather than the motherboard is basic, but in the moment
I jumped to "dead hardware" first. A calm connection check would've saved me
the mild panic.
