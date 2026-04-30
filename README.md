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

> **Note:** Let's get coding! 💻
