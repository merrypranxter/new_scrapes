Alright, let's get into the guts of this thing. I’ve gone through the source over at `ade3.substack.com` and pulled every single technical detail, "dad joke," and hardware spec I could find. If you’re looking to build a "glitch machine" out of a plastic dinosaur, you’re in the right place.

Here is the full, non-summarized breakdown of **How to Make a Glitch Camera** by Ade.

***

# 🛠️ PROJECT REPORT: THE DINO-GLITCH CAMERA
**Source:** [Made by Ade Substack](https://ade3.substack.com/p/how-to-make-a-glitch-camera)  
**Author:** Ade  
**Project Type:** Hardware Circuit Bending / DIY Photography

---

## 1. THE VISION
The goal of this project isn't perfection or megapixels—it's the opposite. It’s about creating a tool for "originality and artistic expression" by intentionally corrupting the data stream between the camera lens and the processing board.

## 2. THE BILL OF MATERIALS (BOM)
If you want to replicate this, don't just buy "a camera." You need specific specs to match the breakout strategy used here.

### **The Core Camera**
*   **Model:** Mgaolo Kids Camera (Dinosaur-themed).
*   **Price:** ~$25 on Amazon.
*   **Variations:** Also available as a unicorn or puppy (Note: pin configurations might vary by model/batch).
*   **Feature Note:** This specific model includes a rear-facing camera.

### **The Hack/Breakout Components**
*   **Breakout Connector:** A FPC/FFC connector breakout board.
    *   **Spec 1:** 24 Pins.
    *   **Spec 2:** 0.5mm pin width.
*   **Ribbon Cable:** A 24-pin, 0.5mm pitch ribbon cable (to connect the camera board back to your breakout).
*   **Jumper Wires:** Colored wires with female-to-female connections (for solderless testing).
*   **Controls:** 
    *   2x Toggle Switches.
    *   2x Potentiometers (for variable glitch intensity).
*   **Enclosure:** 3D Printed Case (Modified version of the [LBVP design](https://github.com/LBVPstuff/Easy-Camera-Circuit-Bend/tree/main/Case%203D%20model)).

### **Tools Needed**
*   Soldering Iron (even if you're "bad at it," as Ade says).
*   Wire cutters.
*   Drill (for the case holes).
*   Zip ties (for final assembly).

---

## 3. THE "SECRET SAUCE": PIN MAPPING
This is where the magic happens. The camera uses a 24-pin ribbon cable to send data from the lens to the screen/storage. By "bending" (crossing) these signals, you get visual artifacts.

### **The Winners**
Through trial and error on the breadboard, Ade identified the most reactive pins:
*   **Pin 1**
*   **Pin 6**
*   **Pin 7**
*   **Pin 8**
*   **Pin 9**
*   **Pin 24**

### **The Risks**
*   **Crashing:** Certain combinations will freeze the camera or force a reboot. If it reboots, you've found a "dead" combination—avoid it.
*   **Color Bars:** If you see a color bar screen immediately, your ribbon cables are likely reversed or misaligned.

---

## 4. STEP-BY-STEP EXECUTION

### **Phase 1: The Dissection**
1.  Open the Mgaolo camera. 
2.  Locate the 24-pin ribbon cable connecting the lens half to the back half.
3.  **Pro Tip:** If you have a microscope and elite soldering skills, you can solder directly to the board. If not (like most of us), use the breakout connector strategy.

### **Phase 2: The Extension**
1.  Connect the lens ribbon cable to your breakout board.
2.  Run the new 24-pin ribbon cable from the breakout board back to the original camera mainboard.
3.  Test it now! Ensure the camera still takes "normal" photos before you start crossing wires.

### **Phase 3: The Glitch Hunt**
1.  Using the female-to-female jumper wires, start touching different pin outputs on your breakout board.
2.  Watch the screen for:
    *   Pixel dragging.
    *   Color shifts.
    *   Static/Noise.
    *   Total frame corruption.
3.  Once you find combinations you like, note the pin numbers.

### **Phase 4: Final Hardware Build**
1.  **Soldering:** Solder your chosen pins (specifically combinations of 1, 6, 7, 8, 9, and 24) to your switches and potentiometers.
2.  **The Case:** Ade used a 3D printed case but shortened the height.
3.  **Hole Drilling:** Drill ports for:
    *   2 Switches (Top).
    *   2 Knobs/Potentiometers (Sides).
    *   1 Tripod mount (Bottom).
4.  **Microphone Recovery:** Don't forget the mic! It’s usually attached to the front of the original case. Snip it and re-mount it between your new switches.
5.  **Assembly:** Use zip ties to secure the two halves of the 3D printed case.

---

## 5. ADDING THE "RIZZ" (AESTHETICS)
Ade’s "branding" steps:
*   **Lens Hood:** A Coca-Cola bottle cap glued to the front.
*   **Labels:** Use a pencil to mark pin numbers on the case during the build.
*   **Stickers:** For that authentic DIY experimental look.

---

## 6. CAPABILITIES & OUTPUT
*   **Still Photos:** Produces high-contrast, distorted, and unique glitch art.
*   **Video:** Hell yeah, it takes video too. The glitches translate into motion for some truly trippy footage.

---

## 7. EXTERNAL ARCHIVE & RESOURCES
Ade points to three specific "masters" of this craft if you get stuck:
1.  [Mike Sisk’s Video](https://youtu.be/iJslS16d5Ug) - For the fundamentals of circuit bending.
2.  [LBVP’s Connector Strategy](https://youtu.be/pKovYRPuqpo) - Detailed look at using the 24-pin breakouts.
3.  [Get Circuit Bent’s Breakout Board](https://youtu.be/yab0vFGAiJ8) - For a more custom PCB approach.
4.  [GitHub Repo (LBVPstuff)](https://github.com/LBVPstuff/Easy-Camera-Circuit-Bend) - Contains the 3D files and the most accurate pinout diagrams available.

***

### **Scrapes McGee’s Final Take:**
This is one of the cleanest "messy" hacks I’ve seen. The 24-pin 0.5mm breakout is the crucial bit—without that, you're looking at soldering pads the size of a dust mite. Nailed it.

**REPO BACKUP:** I'm pushing this full report to `merrypranxter/new_scrapes/2024-04/dino-glitch-camera-manual.md` right now. 

Need this in a CSV for parts sourcing or a JSON for a project manager? Just say the word.