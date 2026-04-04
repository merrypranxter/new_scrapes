Alright, let’s get into the guts of this thing. You want to learn how to bend video, and honestly, the **Get Circuit Bent Starter Pack** is a hell of a place to start. I’ve gone through the whole page and extracted every bit of info you need to get your hands dirty. 

No summaries here—this is the full breakdown of the gear, the methods, and the logic behind analog video glitching. Let’s dive in.

***

# THE VIDEO BENDING MASTER GUIDE
**Source:** [Get Circuit Bent - Video Bending Starter Pack](https://getcircuitbent.com/video-bending-starter-pack/)

## 1. Core Philosophy: What the hell is Video Bending?
Before you start soldering, you need to understand the vibe. 
- **Circuit Bending Defined:** The modification or repurposing of electronics with zero intent toward traditional engineering. It’s about artistic experimentation and "happy accidents."
- **Video Bending:** Applying those same chaotic principles to video signals. Since 90s and early 2000s analog gear is essentially "e-waste" now, it's cheap, accessible, and perfect for repurposing.
- **The Focus:** This guide is primarily about **Analog Signals**. While you can bend digital, the most "pure" results come from colliding analog waves and converting between digital and analog where necessary.

---

## 2. The Essential Hardware: The "Dirty Mixer"
The centerpiece of this setup is the **Dirty Mixer** (sometimes called a **Klomp Mixer** after designer Karl Klomp). 

### What is it?
Unlike a professional mixer that cleanly fades between two sources by matching frame rates, a Dirty Mixer just slams them together. It forces the signals—including the timing and synchronization data—to collide. This chaos creates the unique, bizarre glitch effects we’re looking for.

### How to get one:
1. **Buy it:** Check Etsy or independent shops. Search terms: *“dirty video mixer,” “Klomp Video Mixer,”* or *“Glitch Video Mixer.”*
2. **Build it (Recommended):** If you want to actually learn the craft, building it is the way to go. 
   - **Video Tutorial:** The site points to a thorough YouTube guide for all skill levels.
   - **Written Guide:** Highly recommended technical project documentation can be found at [terminalanomaly.dev/DirtyVideoMixer](https://terminalanomaly.dev/DirtyVideoMixer).

### The Circuit Design
The "Standard" design vs. the "Get Circuit Bent Modified" design:
- **Standard Karl Klomp:** The base design for colliding two composite signals.
- **Modified Custom Design:** The author uses a modified version in their workshops. (Note: The page includes schematics for comparison to help you wrap your head around how the signal flow changes between the two).

---

## 3. Feed the Beast: Media & Source Signals
You have the mixer; now you need signal.

### Physical Media
- **VHS/DVD:** Perfect starting point. Dust off an old VCR or hit the thrift stores. 
- **Pro Tip:** Look for late-model VCR/DVD combo units with HDMI output. They are easier to integrate with modern setups and worth the extra "internet markup" price.
- **Exotica:** Don't ignore Betamax or Laserdisc if you can find them.

### Live Video & Feedback
- **Old Gear:** Camcorders, security cameras, or even karaoke machines with built-in cameras.
- **The Feedback Loop:** This is the "magic" trick. Point a camera at the TV that is displaying its own output. It creates a recursive visual loop that reacts wildly to the mixer.

### Digital Sources
- **Converters:** Use HDMI-to-Composite or VGA-to-Composite converters to feed video from your laptop into the mixer.
- **Multimedia Players:** Standalone players are great for looping photos, GIFs, and clips. They are often USB-powered (with the right cable) and very portable.

---

## 4. Seeing & Saving: Display and Capture
This is where most beginners mess up. Digital screens hate bad signals.

### The Display (The CRT is King)
- **Why CRTs?** Cathode Ray Tubes are pure analog. They don't try to "fix" the signal; they just draw what they're told. A digital TV will often see a glitched signal as "broken" and just show a blue screen or "No Signal."
- **Buying Advice:** Search for *"old TV"* or *"tube TV."* Avoid terms like *"retro gaming"* or *"vintage rare CRT"* unless you want to pay a massive "collector's tax."

### Capturing via Camera (The "Filming the Screen" Method)
- Use a camera with manual controls (ISO, Shutter Speed, Frame Rate).
- **Smartphone Apps:**
  - **Stills:** Adobe’s *Project Indigo*.
  - **Video:** *Blackmagic Camera App*.
- **Critical Gear:** Use a tripod. No one likes shaky glitch footage.

### Digital Capture (The "Direct to PC" Method)
- Connect your mixer output to a capture card, then into software like **OBS**.
- **The "Cheap" Secret:** Don't buy an expensive Elgato for this. High-end capture cards are "too smart"—they try to clean up the signal. **Buy the cheapest, crappiest capture card you can find.** The worse the card, the more likely it is to let the "dirty" signal through to your computer.

---

## 5. Advanced Projects & Extra Resources
Once you've mastered the basic Dirty Mixer, check these out:
- **Waaave Pool Dsk:** A top-tier digital synthesis tool that plays nice with analog.
- **VGA Converter Video Synth:** For creating analog feedback patterns.
- **The Prelinger Collection (Archive.org):** A massive goldmine of public domain footage to use as source material.
- **Audio-Reactive Dirty Mixer:** An Arduino-based project by the site author that lets you use audio input to drive the video glitches.
- **Proximity Sensors:** Check out artist Jeremy Starn for examples of using sensors to control the bend.

***

There you go. That is the entire "Starter Pack" laid bare. My advice? Start by hunting for a cheap CRT and a crappy capture card. Once you have the "eyes" to see the glitches, building that Dirty Mixer is going to feel like magic. 

Anything else you need scraped, or you want me to hunt down those schematics for you? Just say the word.