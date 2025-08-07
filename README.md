# 💬 SVG Texting Bubble Animation

A lightweight, animated SVG snippet that simulates a **typing indicator** followed by a **text message**—perfect for portfolios, GitHub profiles, or landing pages.

---

## ✨ Features

- Pure SVG – no JavaScript or libraries needed
- Typing animation with animated dots
- Message reveal section
- Fully customizable timing, text, and layout
- Easy to embed anywhere

---

## 🧩 Code Snippet
```html
<!-- TYPING BUBBLE (appears while "typing") -->

<g transform="translate(10, 170)" class="typing-5">
  <!-- Main speech bubble shape -->
  <rect x="8.27246" width="69.7276" height="42" rx="20.9774" class="bubble" />
  
  <!-- Small tail circles that make the bubble look like it's coming from a speaker -->
  <circle cx="13.591" cy="33.091" r="7.68185" class="bubble" />
  <circle cx="3.54547" cy="41.9547" r="3.54547" class="bubble" />

  <!-- Typing dots: fade in and out like iMessage -->
  <!-- Dot 1 -->
  <circle cx="27.4778" cy="20.9773" r="5.02275" fill="#999999">
    <animate 
      attributeName="opacity" 
      values="0.5;1;0.5"        <!-- fade in/out -->
      dur="1s"                  <!-- duration of 1 animation cycle -->
      repeatCount="indefinite" <!-- keep looping -->
    />
  </circle>

  <!-- Dot 2, starts later -->
  <circle cx="42.8411" cy="20.9773" r="5.02275" fill="#999999">
    <animate attributeName="opacity" values="0.5;1;0.5" dur="1s" begin="0.2s" repeatCount="indefinite" />
  </circle>

  <!-- Dot 3, starts even later -->
  <circle cx="58.2054" cy="20.9773" r="5.02275" fill="#999999">
    <animate attributeName="opacity" values="0.5;1;0.5" dur="1s" begin="0.4s" repeatCount="indefinite" />
  </circle>
</g>
```
## 🎨Customization
| Element        | You Can Change...                                |
| -------------- | ------------------------------------------------ |
| `<text>`       | The actual message inside the bubble             |
| `cx`, `cy`     | Dot and bubble positions                         |
| `dur`, `begin` | Animation speed and delay                        |
| `fill`         | Dot color (hex or CSS color name)                |
| `display`      | Use CSS to toggle `.typing-5` and `.msg-5` views |

## 💡 How to Use
Paste the full code into your a github file ending in .svg

Preview and iteratively customize to your liking

You can showcase it on your profile by copying what I did with your own username and path instead

## 🙌 Final Thoughts
This SVG texting bubble is a fun, creative way to express your personality and technical flair—whether you're showcasing your portfolio, adding some motion to your GitHub profile, or simply experimenting with SVGs.

Feel free to fork, remix, and make it yours.
* If you use it or improve it, tag me or drop a ⭐️ on the repo!


