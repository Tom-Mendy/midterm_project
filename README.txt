## **README — Third-Person Combat Simulation**

### **Design Decisions**

I chose to implement the enemy AI using a **Behavior Tree and Blackboard system** instead of simple Blueprint logic. This made the AI more modular and easier to extend, especially for handling multiple states such as retreating, firing, and roaming.

I implemented the **line-of-sight system using LineTrace** from the enemy’s MuzzlePoint to the player instead of relying on distance only. This ensures that enemies only shoot when the player is actually visible.

For movement, I used a **retreat system based on vector calculation** to maintain distance from the player. This respects the requirement of keeping at least 1000 units away while keeping the implementation simple and efficient.

---

### **Known Bugs / Limitations**

* Roaming for the enemies isn’t smooth.
* Enemy firing timing is basic and can feel slightly predictable since it uses a fixed delay.

---

### **Extra Features**

---
