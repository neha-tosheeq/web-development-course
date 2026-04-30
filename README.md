# 📚 CSS Learning Notes




# Selector   

                
## 🛠️ Syntax of CSS
CSS mein hum **Property** aur **Values** ka istemal karte hain.
- **Property:** Jo feature change karna ho (e.g. `color`).
- **Value:** Jo tabdeeli lani ho (e.g. `green`).

### Example:
```css
h1 {
    color: green;
    font-family: "Times New Roman";
    text-align: center;
}
```

---

## 🔗 3 Ways to Link HTML with CSS
1. **Inline CSS:** HTML tag ke andar `style` attribute use karna.
2. **Internal CSS:** `<head>` tag ke andar `<style>` tag use karna.
3. **External CSS:** Alag se `.css` file bana kar link karna.

---

## 🎯 Selectors in CSS
Selectors se hum batate hain ke kis element ko style karna hai:


| Selector Type | Syntax | Example |
| :--- | :--- | :--- |
| **Tag Selector** | `h1 { }` | `p { color: blue; }` |
| **Class Selector** | `.className { }` | `.my-text { font-size: 20px; }` |
| **ID Selector** | `#idName { }` | `#main-header { color: red; }` |

---

## 🎭 Pseudo-classes & States
Elements ki different states ko style karne ke liye:
- **:hover** - Jab mouse element ke upar ho.
- **:visited** - Jab link par click ho chuka ho.
- **::first-line** - Paragraph ki pehli line ko target karne ke liye.

```css
/* Example for Hover */
a:hover {
    color: brown;
    text-decoration: underline;
}
```
---
## 🏗️ Advance Selectors

### 1. Combinator Selector
Iska istemal parent element ke andar kisi specific child element ko select karne ke liye hota hai.
- **Example:** `div p { color: gray; }` (Ye sirf un paragraphs ko select karega jo div ke andar hain).

### 2. Universal Selector (`*`)
Agar humein page ke **saare elements** ko ek saath select karke koi style dena ho (jaise margin ya padding khatam karni ho), to hum Universal Selector use karte hain.

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```

---

## 🔗 HTML Tags Info
- **`<a>` Tag:** Iska matlab hai **Anchor Tag**. Ye ek website se doosri website ya ek page se doosre page par jane ke liye links banane ke kaam aata hai.
---

# 🎨 Properties in CSS

Ye notes aapko basic styling aur text formatting mein madad dein ge.

---

  
###  1.🌈 Colors
CSS mein color dene ke mukhtalif tarike hain:
```css
*   **Names**: `red`, `blue`, `hotpink`.
*   **Hex**: `#ffffff` (White), `#000000` (Black).
*   **RGB**: `rgb(255, 255, 255)`.
*   **RGBA**: `rgba(0, 0, 0, 0.5)` (Is se rang ko transparent/halka kiya ja sakta hai).
```
---

### 2. 🖼️ Background Styling
Background ko control karne ki properties:
```css
*   **`background-color`**: Element ke piche rang bharne ke liye.
    > `background-color: yellow;`
*   **`background-image`**: Piche photo lagane ke liye.
    > `background-image: url('image.jpg');`
*   **Helper Properties**:
    *   `background-size: cover;` (Photo ko poori jagah par fit karta hai).
    *   `background-repeat: no-repeat;` (Photo ko baar baar repeat hone se rokta hai).
```
---

### 3. 📝 Text Formatting & Styling
Text ki look aur position set karne ke liye:
```css
*   **Text Color**:
    *   `color: blue;` (Sirf likhay huye text ka rang badalta hai).
*   **Text Alignment**:
    *   `text-align: center;` (Text ko darmiyan mein lane ke liye).
    *   `text-align: right;` (Right side ke liye).
    *   `text-align: left;` (Default left side).
*   **Text Transform** (Likhai ka style):
    *   `text-transform: uppercase;` (Saray letters BADE karne ke liye).
    *   `text-transform: lowercase;` (Saray letters chote karne ke liye).
    *   `text-transform: capitalize;` (Har word ka pehla letter bada karne ke liye).
```
---

### 4. 🔡 Fonts (Likhai ka Design)
*   **`font-family`**: Font ka naam (e.g., `'Arial'`, `'Poppins'`, `sans-serif`).
*   **`font-size`**: Text kitna bada dikhega (e.g., `20px`, `2rem`).
*   **`font-weight`**: Text ko kitna mota (bold) karna hai (e.g., `bold`, `400`, `700`).
*   **`font-style`**: Text ko teercha karne ke liye (`italic`).

---



