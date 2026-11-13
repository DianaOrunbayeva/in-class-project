# Web Communication Exam Prep & Teacher Questions

> **Tip:** Keep this file on your desktop or phone to review before class. Do not include this file inside the `in-class-project/` folder if you zip and submit it!

---

## Part 1: HTML & Page Structure

### 1. "Why did you use `<header>`, `<nav>`, `<main>`, and `<footer>` instead of regular `<div>` tags?"
* **What to say:**  
  > *"Because they are semantic tags. A `<div>` is just an empty box that has no meaning, but `<header>`, `<nav>`, and `<footer>` tell the browser, search engines, and screen readers exactly what each section does."*
* **What it means:** It makes the code clean, professional, and accessible.

---

### 2. "Why is there only one `<h1>` on the entire page?"
* **What to say:**  
  > *"Best practice for SEO and accessibility is to have only one `<h1>` per page for the main headline ('Make stories that stand out'). All the other section titles use `<h2>` or `<h3>` to create a clear hierarchy."*
* **What it means:** Think of a newspaper: there's only one main headline at the top, and smaller sub-headlines below.

---

### 3. "How do the menu links jump down the page (like clicking 'Useful links')?"
* **What to say:**  
  > *"They are anchor links. The menu link has `href="#links"`, and the target section has `id="links"`. When you click it, the browser automatically scrolls down to that ID."*
* **What it means:** `#links` acts like a bookmark that tells the browser where to jump.

---

### 4. "What is the difference between an `id` and a `class`?"
* **What to say:**  
  > *"An `id` is unique and can only be used once on a page (like `id="about"`). A `class` can be reused on multiple elements that share the same style, like `class="section"` or `class="two-columns"`."*
* **What it means:** `id` is a unique name tag; `class` is a category tag.

---

### 5. "Why do your external links have `target="_blank"` and `rel="noopener"`?"
* **What to say:**  
  > *"`target="_blank"` opens external university pages in a new tab so visitors don't lose our landing page. `rel="noopener"` is a standard security practice for external links opened in new tabs."*
* **What it means:** It keeps the user on your site while opening outside pages in a separate tab safely.

---

### 6. "Why do all your `<img>` tags have `alt` text?"
* **What to say:**  
  > *"For accessibility and SEO. If an image fails to load, or if a visually impaired student uses a screen reader, the alt text describes what is in the photo."*
* **What it means:** It's a text backup describing the picture.

---

### 7. "Why did you use `youtube-nocookie.com` for the video embed?"
* **What to say:**  
  > *"It's YouTube's privacy-enhanced mode. It stops YouTube from storing tracking cookies on the visitor's computer until they actually click play."*
* **What it means:** Better privacy for website visitors.

---

### 8. "What are `<dl>`, `<dt>`, and `<dd>` in the programme section?"
* **What to say:**  
  > *"It's a description list. `<dt>` is the term or title (like 'Corporate side' or 'Public side'), and `<dd>` is the description text underneath it."*
* **What it means:**  
  * `dl` = Description List  
  * `dt` = Description Title  
  * `dd` = Description Detail  

---

### 9. "Why did you use `<figure>` and `<figcaption>` for the lab photo?"
* **What to say:**  
  > *"Because HTML provides `<figure>` specifically to group an image with its caption (`<figcaption>`) as a single unit, rather than putting an image and a random `<p>` paragraph."*
* **What it means:** It signals that the caption text directly belongs to the photo.

---

## Part 2: CSS & Visual Styling

### 10. "What are `:root` and `--brand-red` at the very top of your CSS?"
* **What to say:**  
  > *"Those are CSS custom properties (variables). I saved the official Unimi red hex code (`#a6192e`) as `--brand-red` so I could easily reuse it across headers, buttons, and borders without retyping the code every time."*
* **What it means:** It's like saving a color to a shortcut name so you can reuse it everywhere.

---

### 11. "What does `* { box-sizing: border-box; }` do?"
* **What to say:**  
  > *"It makes layout math predictable. It includes padding and borders inside an element's total width and height, so adding padding won't accidentally break the layout or push boxes outside the screen."*
* **What it means:** If a box is 300px wide and you add 20px padding, it stays 300px instead of expanding to 340px.

---

### 12. "How did you turn the computer lab photo black and white?"
* **What to say:**  
  > *"With one line of CSS: `filter: grayscale(100%);` on the image. In class we noted that the bright blue computer screens in that photo were distracting, so the grayscale filter makes the section look much cleaner and more professional."*
* **What it means:** An instant black-and-white filter applied via CSS without needing Photoshop.

---

### 13. "What does `object-fit: cover;` do on the Torre Velasca photo in the hero?"
* **What to say:**  
  > *"It makes the image fill its container completely without stretching or distorting the photo proportions. It crops the edges cleanly like a background image."*
* **What it means:** The photo looks sharp and natural instead of being squished or stretched.

---

### 14. "How did you connect the Google Fonts (Merriweather & Source Sans 3)?"
* **What to say:**  
  > *"I included the `<link>` tags from Google Fonts in the `<head>` of the HTML, and then applied `font-family: Merriweather, Georgia, serif` for headings and `font-family: 'Source Sans 3', sans-serif` on the body."*
* **What it means:** Downloaded clean online fonts directly through Google.

---

### 15. "How does the button hover animation work?"
* **What to say:**  
  > *"The `.btn-apply` class has `transition: 0.2s ease;`. When the mouse hovers over it (`.btn-apply:hover`), the background changes to white and text turns red smoothly over 0.2 seconds instead of flashing instantly."*
* **What it means:** It creates a smooth, animated color swap when you hover your cursor.

---

### 16. "How did you make the YouTube video keep its 16:9 shape?"
* **What to say:**  
  > *"I used `aspect-ratio: 16 / 9;` on the iframe. That way, whether on a wide desktop screen or a narrow phone screen, the video always keeps the correct widescreen proportions without black bars."*
* **What it means:** It prevents the video player from getting crushed or warped.

---

## Part 3: Flexbox & Mobile Responsiveness

### 17. "What is Flexbox and where did you use it?"
* **What to say:**  
  > *"Flexbox (`display: flex`) is a CSS layout tool for aligning elements in rows or columns. I used it for the top navigation bar, the two-column hero section, the two-column content sections, and the footer links."*
* **What it means:** It’s the modern way to arrange boxes next to each other cleanly.

---

### 18. "What does `flex-wrap: wrap;` do?"
* **What to say:**  
  > *"It tells flex items that if there isn't enough horizontal room on the screen, they should wrap onto the next line instead of shrinking or overflowing off the edge."*
* **What it means:** Side-by-side boxes can drop under each other when the screen gets narrower.

---

### 19. "How does your mobile media query work?"
* **What to say:**  
  > *"At the bottom of the CSS, I wrote `@media (max-width: 768px)`. When the screen width is 768px or smaller (tablets and phones), it stacks the navigation items and adjusts headings and padding so the page is easy to read without zooming."*
* **What it means:** Special rules that kick in only on smaller screens.

---

### 20. "How did you test the website?"
* **What to say:**  
  > *"I tested it in the browser (Firefox and Chrome) using Developer Tools in Responsive Design Mode, checking how the layout shifts across desktop, tablet, and mobile widths."*
* **What it means:** Resized the screen in the browser to make sure nothing breaks on phones.

---

## Part 4: Web Communication & Design Strategy

### 21. "Why did you choose red as the accent color?"
* **What to say:**  
  > *"Because `#a6192e` is the official institutional color of Università degli Studi di Milano (La Statale). It keeps the page aligned with university branding while giving the hero section strong visual impact."*

---

### 22. "Why did you pair a serif font with a sans-serif font?"
* **What to say:**  
  > *"We used Merriweather (serif) for headings to give an academic, authoritative feel, and Source Sans 3 (sans-serif) for body text and navigation because clean sans-serif text is much easier to read quickly on screens."*

---

### 23. "Why did you organize the quick links into Before, During, and After?"
* **What to say:**  
  > *"It matches the user journey. Prospective students immediately see admission and syllabi, current students can quickly find schedules and internships, and graduating students can find career and contact info."*
