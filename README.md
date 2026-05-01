# 📚 CSS Learning Notes

# Selector   

## 🛠️ Syntax of Selector
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
# 📕 Understanding Box Model(L3)
 ## 📋 Document Object Model (DOM)
 ### *`Parent`* -> *`Child`* -> *`Siblings`*
 
| HTML Side | Action | CSS Side |
| :--- | :---: | :--- |
| Load HTML | ➔ | Load CSS |
| Parse HTML | ➔ | Parse CSS |
| **DOM Tree** | ➔ | **Attach Style** |
| | **DISPLAY** | |
|
# 🎲 Units in CSS
- A CSS Unites determined the size of a property you's setting for an element or its content.
---
## Types:
1. Relative
2. Absolute
---
### Relative Units:
- Relative length Units are related to something else,Perhaps the size of the parent element's font or the size of the viewport.


Relative length units kisi doosri cheez (jaise parent element ya viewport) ke mutabiq size set karti hain.


### 🔹 Important Relative Units

*   **`%` (Percentage)**: Ye apne **parent element** ke size ke mutabiq hota hai.
*   **`em`**: Ye us element ke **apne font-size** ke mutabiq hota hai (e.g., 2em ka matlab hai font-size se double).
*   **`rem`**: Ye **Root element** (`<html>`) ke font-size ke mutabiq hota hai.
*   **`vw` (Viewport Width)**: Viewport (screen) ki chorai ka 1%.
*   **`vh` (Viewport Height)**: Viewport (screen) ki lambai ka 1%.
*   **`vmin`**: Viewport ki choti dimension (width ya height mein se jo chota ho) ka 1%.
*   **`vmax`**: Viewport ki badi dimension ka 1%.

---
### Absolute Unit:

- Absolute units wo fixed units hoti hain jo screen size ya parent element ke mutabiq change nahi hotin. Ye hamesha utni hi rehti hain jitni aapne likhi hon.


### 🔹 List of Absolute Units

*   **`px` (Pixels)**: Sab se zyada use hone wali unit. (1px = 1/96th of 1 inch).
*   **`cm` (Centimeters)**: 1cm = 96px / 2.54.
*   **`mm` (Millimeters)**: 1mm = 1/10th of 1cm.
*   **`in` (Inches)**: 1in = 96px = 2.54cm.
*   **`pt` (Points)**: Zyada tar printing mein kaam aata hai. (1pt = 1/72 of 1 inch).
*   **`pc` (Picas)**: 1pc = 12pt.

---
# 📤 Box Model
```css
1. Content Aera (Text).
2. Padding (Top,Right,Left,Button). 
    -> Content ka Surrounding Space. 
    -> Include background Colour.
    -> Fixed Don't Change the background Colour.
3. Border (Top,Right,Left,Button). 
    -> Include background Colour.
4. Margin (Top,Right,Left,Button). 
   -> Don't Include background. Colour.
```
---

## 📘 CSS Core Concepts (L4)

Browser CSS ko teen main cheezon ki bunyaad par apply karta hai:

### 1. Cascading 🌊
CSS ka matlab hi **Cascading Style Sheets** hai. Iska asool ye hai ke agar do rules aik hi element ke liye hon, to jo **sab se aakhir mein** likha hoga, wahi apply hoga.

### 2. Specificity ⚖️ (Power Scale)
Agar rules alag alag jagah likhay hon, to browser "Power" check karta hai:
- **(0,1,0,0) ID Selector (`#header`):** Sab se zyada power.
- **(0,0,1,0) Class Selector (`.heading`):** Darmiyani power.
- **(0,0,0,1) Tag Selector (`h1`):** Sab se kam power.

->   Ye sab scores ko maat de deta hai aur apna style apply karwata hai.

### 3. Inheritance (Wirasat) 👨‍👩‍👧
Child elements apne parents ki properties (jaise `color`) hasil karte hain. Inhein control karne ke liye ye keywords use hote hain:
- `initial`: Default browser value par le jata hai.
- `inherit`: Parent ki value hasil karne par majboor karta hai.
- `unset`: Property ko uski natural state par le jata hai.

---

















            




