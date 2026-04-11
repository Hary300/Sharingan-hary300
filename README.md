# 👁️ Sharingan Animation Practice

A simple front-end practice project inspired by the Sharingan eye design. This project focuses on experimenting with **CSS Grid, animations, keyframes, transitions, and rotation effects**.

Live Demo: https://sharingan-hary300.vercel.app/

---

## 🚀 About the Project

This project was created as a **practice exercise** to improve understanding of modern CSS techniques such as layout positioning and animations.

The main focus is on how visual elements can be created and animated using only **HTML and CSS** without any JavaScript.

---

## ✨ Features

- 🎯 CSS Grid layout
- 🔄 Rotation animation using `keyframes`
- 🎨 Smooth transition effects
- 🖱️ Hover interactions
- 👁️ Inspired Sharingan-style design
- ⚡ Pure HTML & CSS (no frameworks)

---

## 🛠️ Built With

- HTML
- CSS
- CSS Animations (`@keyframes`)
- CSS Transitions
- CSS Grid

---

## 🧠 What I Learned

Through this project, I practiced:

- How to structure layouts using CSS Grid
- Creating smooth animations with `@keyframes`
- Using `transform: rotate()` for motion effects
- Combining hover states with animations
- Improving visual design using pure CSS

### ⚠️ Important Lesson: Animation State Behavior

I also learned that **CSS animation state can override element behavior**.

For example:

- If an element is animated using `forwards` fill mode (e.g. rotate 360deg),
  the element will **stay at its final state (360deg)**.
- When trying to apply a `hover` animation afterward (e.g. rotate again),
  it may not work because the element is already at the final state.

This happens because the element's **computed state is not reset**.

### 💡 Better Approach

Instead of relying on `animation-fill-mode: forwards`, it is often better to:

- Let the animation return to its original state (0deg)
- Avoid locking the final state when you still need interaction
- Use `transition` or reset-friendly animations for hover effects
