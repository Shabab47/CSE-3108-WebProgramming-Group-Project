# CSE-3108-WebProgramming-Group-Project
# 🌍 Geo-Farm: Real-World Weather Farming Simulator

A **2D real-time farming simulator** where your environment, difficulty, and crop health are dynamically driven by live, real-world location and weather data.

---

## 🚀 About the Project

**Geo-Farm** connects virtual simulation with real-world elements. Players manage a rectangular plot of land, battle local weather shifts, and practice financial management to expand their assets. The core twist? If it is raining, scorching, or experiencing a drought in your chosen real-world city, your virtual crops will feel the impact instantly.

---

## 🛠️ Tech Stack & Base APIs

The game engine relies on three external integrations to drive gameplay mechanics:

* **Weather API:** Pulls live meteorological data to create real-time farming difficulty based on your chosen location.
* **Time API:** Tracks precise regional time zones to calculate real-world crop growth intervals.
* **Map API:** Allows players to pick any real-world coordinate or city across the globe to establish their farm.

---

## 🎮 Base Game Mechanics

### 👨‍🌾 Core Loop & Economy
1. **Plough & Plant:** Spread seeds across a muddy, rectangular plot. This triggers a custom farmer animation sprite (2-3 frames, backside view) visible only during seeding.
2. **Nurture:** Keep your crop health optimized by carefully balancing a live **Heat Meter** and **Water Meter**. Excess water from prolonged rain or over-pumping will damage the harvest.
3. **Harvest (n Hours):** Reap fully matured crops after actual, real-world hours have elapsed based on the local time API.
4. **Trade:** Sell your yield at the Market for gold coins. Good care results in high-quality yields and bigger profits, while neglect, droughts, or pests result in lower quality and financial loss.
5. **Expand & Equip:** Reinvest your gold coins into the shop menu to buy:
   * **Seeds:** To grow more crops.
   * **Scarecrows:** To ward off crop-eating crows across a limited, specific radius.
   * **Water Pumps & Oil:** Fuel the pump with oil to manually irrigate a specific area size during local droughts.
   * **Land:** Expand your farming assets by purchasing more land.

### 🎨 Visuals & Animation States
The game features a top-down or slightly tilted 2D perspective (similar to Clash of Clans) with specific visual states:
* **Grassy background** with a muddy, rectangular farming field.
* **5 Crop Growth Levels:** Empty Mud ➔ Small Green Saplings ➔ Mid-size Growth ➔ Full Size (Green) ➔ Mature (Golden Harvest).
* **Unique Threat Sprites:** Dedicated graphics for rain-damaged crops, drought-killed crops, and crow-eaten crops.
* **Animated Water Pump:** A 3-frame animation system tracking "No Pumping", "Pumping Frame 1", and "Pumping Frame 2".

---

## 🔮 Future Roadmap

These advanced systems are planned for future expansions once the base game mechanics are fully stable:

### 🎨 Visual & Asset Upgrades
* Implement high-fidelity graphical assets and fluid entity animations.
* Expand the shop inventory with more items and diverse plant species.

### 🐛 Enhanced Gameplay Challenges
* Introduce complex plant diseases and advanced crop needs.
* Introduce new types of crop-stealing enemies and pests.

### ⚙️ Automation & Equipment Tiering
* Add a worker hiring system to delegate manual farming tasks.
* Introduce different models of water pumps.
* Add heavy machinery and tools for high-efficiency reaping, complete with a machine repair/maintenance system.

### 📈 Dynamic Macro-Economy
* Build a fully simulated **Supply & Demand Market Engine** where crop pricing dynamically fluctuates based on seasonal demands, location data, local traditions, and unexpected natural calamities.
