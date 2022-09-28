# Rollenverständnis - Mensch - Maschine (KI)

<div style="position: absolute; width: 70%; left: 15%">
<img src="./public/img/wissenstreppe.png" />
</div>

<div style="position: absolute; bottom: 20px; right: 20px; font-size: 50%; color: #999">
<a href="https://openai.com/dall-e-2/" target="_blank">angelehnt an Wissenstreppe nach North (2011)
</a>
</div>

---
preload: false
---

# Rollenverständnis - Mensch - Maschine (KI)

<div style="position: absolute; width: 70%; left: 15%">
<img src="./public/img/wissenstreppe.png" />
</div>

<div style="position: absolute; width: 70%; left: 15%">
    <div
        v-motion
        :initial="{ opacity: 0, x: -600, y: 100, scale: 0.75 }"
        :enter="{ x: -120, y: 50, opacity: 1, transition: { duration: 0, delay: 0 } }"
    >
        <img
            src="./public/img/circle1.png"
        />
        <div style="transform: rotate(-15deg);">
            <h2
                style="transform: translate(300px, -100px);"
            >Maschine</h2>
        </div>
    </div>
    <div
        v-motion
            :initial="{ opacity: 0, x: 600, y: -600, scale: 0.75 }"
            :enter="{ x: 120, y: -450, opacity: 1, transition: { duration: 0, delay: 0 } }"
    >
        <img
            src="./public/img/circle2.png"
        />
        <div style="transform: rotate(-15deg);">
            <h2
                style="transform: translate(400px, -100px);"
            >Mensch</h2>
        </div>
    </div>
</div>

<div style="position: absolute; bottom: 20px; right: 20px; font-size: 50%; color: #999">
<a href="https://openai.com/dall-e-2/" target="_blank">angelehnt an Wissenstreppe nach North (2011)
</a>
</div>