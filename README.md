# Orbital-Snap-2D-game-mobile
Mobile game 2d 

<img width="1024" height="572" alt="image" src="https://github.com/user-attachments/assets/361a72f5-8ae4-4714-a050-9dc1dd17abe9" />


🕹️ Step 1: Understanding the 2 Fixed Tracks
The game is based on extremely precise geometry centered around the middle of the screen:
Inner Track (Track 0): Tight radius (70 px). Fast angular rotation, short reaction time.
Outer Track (Track 1): Wide radius (140 px). High linear speed, unobstructed field of view.
Your white orb orbits indefinitely around the center in a continuous, frictionless clockwise rotation.
Translated with DeepL.com (free version)

Step 2: The Single Action (The Instant Snap)
Control comes down to a single universal command (tap the screen, click the mouse, or press the spacebar):
A single tap instantly teleports the orb between the inner and outer tracks.
No sliding, no latency: the orbit change occurs in a single sub-frame and produces a micro-elastic deformation (squish & stretch) accompanied by a burst of white particles.
Translated with DeepL.com (free version)

Step 3: Identify the Expanding Rings
Circular waves radiate from the center and grow larger toward the edges of the screen:
Cyan Ring (Target): You must position yourself on its path just as it crosses your beam. The impact shatters it, triggers a freeze-frame (32 ms hit-stop), and causes the screen to shake.
Red Ring (Deadly Obstacle): Any contact with your orb results in immediate destruction (SHATTERED). You must switch to the opposite track before impact.

Step 4: Build the Multiplier & Trigger “Near Misses”
Performance and the high score depend on taking risks:
Exponential Combo: Each cyan target destroyed in a row increases the multiplier (x2, x3, x4...). Letting a cyan ring pass beyond the outer track immediately breaks the combo.
“CLOSE!” Bonus: Switching orbits within 200 ms of a red ring on the track you just left counts as a Near Miss: massive points and a micro-jolt of reward.
