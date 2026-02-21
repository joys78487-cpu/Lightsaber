# 🔴 Sith Saber – Interactive CSS Lightsaber

An interactive **Sith-style red lightsaber** built using pure **HTML, CSS, and JavaScript**.  
Click the button to ignite or retract the blade with a smooth animation and glowing flicker effect.

Inspired by the dark side energy from *Star Wars* — especially the intense red blades seen in **_Star Wars: Episode III – Revenge of the Sith (2005)_**.

---

## 🚀 Features

- ⚡ Smooth ignition animation using CSS transforms  
- 🔥 Animated red glow flicker effect  
- 🎯 Centered layout using Flexbox  
- 🖱 Simple toggle button interaction  
- 💡 No external libraries required  

---

## 📁 Project Structure

```
sith-saber/
│
├── index.html
└── README.md
```

Everything (HTML, CSS, JS) is written inside a single HTML file.

---

## 🧠 How It Works

### 1️⃣ Blade Animation

The blade is initially hidden using:

```css
transform: scaleY(0);
transform-origin: bottom;
```

When activated, it scales vertically:

```css
transform: scaleY(1);
```

This creates a **realistic ignition effect from bottom to top**.

---

### 2️⃣ Glow & Flicker Effect

The glow is created using layered `box-shadow`:

```css
box-shadow:
    0 0 10px #ff0000,
    0 0 20px #ff0000,
    0 0 40px #ff0000,
    0 0 80px #ff0000;
```

The flicker effect uses a keyframe animation:

```css
@keyframes flicker {
    from { ... }
    to   { ... }
}
```

This gives the unstable Sith blade vibe.

---

### 3️⃣ Toggle Function

JavaScript adds/removes the `.active` class:

```javascript
function toggle(){
    document.getElementById("blade").classList.toggle("active");
}
```

That’s it. Simple and clean.

---

## 🎨 Customization Ideas

You can easily modify:

| Change               | How                                 |
| -------------------- | ----------------------------------- |
| Blade Color          | Update gradient + box-shadow colors |
| Blade Height         | Change `height: 65vh;`              |
| Ignition Speed       | Modify `transition` duration        |
| Add Sound            | Use `<audio>` in JS toggle          |
| Add Crackling Effect | Add more flicker variations         |

---

## 🛠 Technologies Used

* HTML5
* CSS3 (Flexbox, Animations, Gradients)
* Vanilla JavaScript

---

## ▶ How to Run

1. Copy the code into a file named:

   ```
   index.html
   ```

2. Open it in any modern browser.
3. Click **IGNITE**.
4. Embrace the dark side.

---

## 🌌 Inspiration

The red blade aesthetic is inspired by Sith lightsabers from  
***Star Wars: Episode III – Revenge of the Sith (2005)***  
novel adaptation by Matthew Stover and the film directed by George Lucas.

---

## 📌 Future Improvements

* Add ignition sound effect
* Add retract animation speed variation
* Add unstable Kylo Ren-style blade
* Mobile vibration support
* Power button glow animation

---

## ⚠ Disclaimer

This is a fan-made educational project created for learning purposes.  
All Star Wars references belong to their respective owners.

---

🔥 *The Force is strong with this one.*
