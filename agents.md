# 🎮 Disgrace — AI Agent Architecture

## 🧠 Overview
A psychological horror chase game driven by dynamic AI entities, escalating tension, and player-induced difficulty.

---

## 🤖 Agents

### 1. Game Engine Agent
- Game loop
- Physics
- Collision

---

### 2. Player Agent
- Movement system
- Camera
- Stamina

---

### 3. Entity AI Agent
Handles ALL entity logic:

Each entity must implement:
- Unique movement algorithm
- Detection rules
- Player interaction
- Scaling difficulty

Includes:
- Nocturne (light-based speed)
- Velour (sound suppression)
- Penance (mistake tracking)
- Lament (slow zones)
- Silhouette (angle visibility)
- Eulogy (ghost paths)
- Crescent (phasing)
- Obsidian (hazards)
- Vespers (patience mechanic)
- Relic (teleport pattern)

---

### 4. Environment Agent
- Lighting system
- Fog
- Maze

---

### 5. UI Agent
- HUD
- Effects
- Feedback

---

### 6. Audio Agent
- Ambient sound
- Entity audio
- Distortion system

---

### 7. Box System Agent
- Stability tracking
- Escape triggers
- Overload logic

---

### 8. Difficulty Agent
- Global scaling
- Entity buffs

---

### 9. Power Agent
- Ability unlocks
- Glitch behavior in overload

---

### 10. Firebase Agent
- Auth
- Save data
- Leaderboards

Fallback:
- localStorage mirror

---

## 🔄 Events
- onEntityCaught
- onEscapeTriggered
- onMistake
- onOverload
- onRunEnd

---

## ⚠️ Core Design Rule
Fear comes from:
- Uncertainty
- Loss of control
- Misinformation

---

## 💀 End Condition
- Total box failure
- Player overwhelmed
