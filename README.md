# EduLaunch Academy - HTML and CSS Final Project

Yeh ek fresh beginner-friendly HTML and CSS project hai. Isme koi old notes ya old project content nahi hai. Project ka goal hai learners ko ek simple academy landing page banana sikhana jisme HTML structure aur CSS styling dono clearly samajh aaye.

## Project Story

Socho ek training academy hai jiska naam `EduLaunch Academy` hai. Academy beginners ko HTML, CSS, aur responsive web design sikhati hai. Academy ko ek simple website chahiye jahan learners courses, weekly plan, aur contact information dekh sakein.

Is project mein hum sirf 2 files use karte hain:

- `index.html` - website ka structure
- `styles.css` - website ka design

## Kaise Run Karna Hai

1. Folder ko VS Code mein open karo.
2. `index.html` file open karo.
3. Right click karo and `Open with Live Server` choose karo.
4. Browser mein website open ho jayegi.
5. Agar Live Server nahi hai, toh `index.html` file ko double click karke browser mein open kar sakte ho.

## Expected Output

Browser mein ek clean academy landing page dikhega. Top par sticky navbar hoga. Hero section mein academy ka main message and button hoga. Popular courses section mein 3 cards honge. Weekly learning plan section mein list hogi. Contact section mein email button hoga. Mobile screen par layout one-column mein convert ho jayega.

## index.html Detailed Explanation

| Code | Simple Hinglish Explanation |
|---|---|
| `<!DOCTYPE html>` | Browser ko batata hai ki yeh HTML5 document hai. Yeh line hamesha file ke top par likhte hain. |
| `<html lang="en">` | HTML document ka root start hota hai. `lang="en"` se browser ko language English pata chalti hai. |
| `<head>` | Head section page ki hidden information rakhta hai, jaise title, meta tags, and CSS link. |
| `<meta charset="UTF-8">` | Text encoding set karta hai. Isse characters properly display hote hain. |
| `<meta name="viewport"...>` | Mobile responsive design ke liye important hai. Page ko device width ke according adjust karne mein help karta hai. |
| `<title>EduLaunch Academy</title>` | Browser tab mein page ka title show karta hai. |
| `<link rel="stylesheet" href="styles.css">` | HTML file ko CSS file se connect karta hai. Agar yeh line missing hogi toh styling apply nahi hogi. |
| `<body>` | Visible page content yahan se start hota hai. |
| `<header class="site-header">` | Website ka top header area. Isme logo and navigation links hote hain. |
| `<div class="container navbar">` | Container content width control karta hai. Navbar class logo and links ko side-by-side arrange karti hai. |
| `<h1 class="logo">EduLaunch Academy</h1>` | Website ka brand name. CSS se iska color and size style hota hai. |
| `<nav class="nav-links">` | Navigation links ka semantic area. Screen readers ko bhi samajh aata hai ki yeh navigation hai. |
| `<a href="#courses">Courses</a>` | Same page ke courses section par le jaane wala link. `#courses` id ko target karta hai. |
| `<main>` | Page ka main content start hota hai. Header and footer ke beech ka important content yahan hota hai. |
| `<section class="hero">` | Website ka first main section. Isme main message and call-to-action button hota hai. |
| `<div class="container hero-grid">` | Hero content ko grid layout mein arrange karne ke liye wrapper. |
| `<p class="tagline">...</p>` | Small highlight line. CSS se uppercase and blue color milega. |
| `<h2>Start your web development...</h2>` | Hero ka main heading. User ko page ka main purpose batata hai. |
| `<a class="primary-button" href="#courses">Explore Courses</a>` | Link hai, lekin CSS se button jaisa dikhega. Click par courses section tak le jayega. |
| `<div class="hero-card">` | Hero ke right side ka information card. Isme next batch details dikhte hain. |
| `<section id="courses" class="section">` | Courses section. `id="courses"` navbar link ke liye target hai. |
| `<div class="course-grid">` | Course cards ko grid columns mein arrange karta hai. |
| `<article class="course-card">` | Har course ek independent card hai, isliye article tag meaningful hai. |
| `<span>01</span>` | Course number show karta hai. CSS se blue bold style milega. |
| `<section id="schedule"...>` | Weekly learning plan section start hota hai. |
| `<ul class="schedule-list">` | Unordered list. Weekly plan points list form mein show karne ke liye use hoti hai. |
| `<li>Day 1...</li>` | List item. Har day ka learning task separate line mein dikhta hai. |
| `<section id="contact"...>` | Contact section. User yahan se academy ko email kar sakta hai. |
| `<a href="mailto:hello@edulaunch.com">` | Email link. Click karne par mail app open ho sakta hai. |
| `<footer class="site-footer">` | Website ka bottom section. Usually copyright ya project credit yahan hota hai. |

## styles.css Detailed Explanation

| CSS Code | Simple Hinglish Explanation |
|---|---|
| `* { box-sizing: border-box; }` | Saare elements par apply hota hai. Padding and border ko width ke andar count karta hai, layout easy hota hai. |
| `body` | Complete page ka base design set karta hai: margin, font, text color, background, and line-height. |
| `margin: 0;` | Browser ka default body space remove karta hai. Page clean edge se start hota hai. |
| `font-family: Arial...` | Website ka font set karta hai. Simple and readable font learners ke liye best hai. |
| `background: #f5f7fb;` | Page ka light background color set karta hai. White cards is par clearly dikhenge. |
| `a { color: inherit; text-decoration: none; }` | Links ka default blue underline remove karta hai. Links parent text color follow karte hain. |
| `.container` | Content ko center and readable width mein rakhta hai. Large screen par content zyada stretch nahi hota. |
| `width: 90%;` | Container screen width ka 90% leta hai, side spacing bachti hai. |
| `max-width: 1120px;` | Large screens par container ko limited width deta hai. |
| `.site-header` | Header ko white background, border, sticky position deta hai. |
| `position: sticky; top: 0;` | Scroll karte waqt header top par visible reh sakta hai. |
| `.navbar` | Flexbox se logo and links ko arrange karta hai. |
| `display: flex;` | Child items ko row mein arrange karne ke liye Flexbox start karta hai. |
| `justify-content: space-between;` | Logo left and links right side push karta hai. |
| `.logo` | Brand name ka color and size set karta hai. |
| `.nav-links` | Navigation links ko row mein arrange karta hai and gap add karta hai. |
| `.nav-links a:hover` | Mouse hover par link blue ho jaata hai. User ko clickable feedback milta hai. |
| `.hero` | First main section ko gradient background and large spacing deta hai. |
| `.hero-grid` | Hero ko two columns mein divide karta hai: left text and right card. |
| `grid-template-columns: 1.4fr 0.6fr;` | Left column ko zyada space and right card ko kam space deta hai. |
| `.tagline` | Small highlight text ko blue, bold, uppercase banata hai. |
| `.hero h2` | Hero heading ko large and strong visual importance deta hai. |
| `.primary-button` | Normal link ko button design deta hai: blue background, white text, padding, rounded corners. |
| `.primary-button:hover` | Button hover par dark blue ho jaata hai. |
| `.hero-card, .course-card, .schedule-box, .contact-box` | Group selector. In sab boxes ko same white card style deta hai. |
| `.section` | Har section ko top-bottom spacing deta hai. |
| `.course-grid` | Course cards ko 3 columns mein arrange karta hai. |
| `repeat(3, 1fr)` | 3 equal columns banata hai. |
| `.course-card` | Har course card ko padding and card design deta hai. |
| `.schedule-box` | Weekly plan section ko grid layout mein arrange karta hai. |
| `.contact-section` | Contact section ka text center align karta hai. |
| `.site-footer` | Footer ko dark background and white text deta hai. |
| `@media (max-width: 768px)` | Mobile responsive rules start karta hai. |
| `flex-direction: column;` | Mobile par navbar ko vertical stack karta hai. |
| `grid-template-columns: 1fr;` | Mobile par grids ko one-column layout mein convert karta hai. |

## Learners Ko Kaise Explain Karna Hai

Pehle students ko HTML file dikhao aur bolo: HTML website ka skeleton hai. Isme content ka order and meaning hota hai. Phir CSS file dikhao aur bolo: CSS website ko design deta hai. Same HTML content CSS ke bina plain dikhega, CSS ke baad professional landing page ban jayega.

Class mein best flow:

1. Pehle `index.html` run karke output dikhao.
2. Phir CSS file mein `.hero` ka background color change karke live output dikhao.
3. Phir `.course-grid` ko `grid-template-columns: 1fr;` karke cards one-column dikhao.
4. Phir browser width kam karke responsive behavior show karo.

Isse learners ko samajh aayega ki CSS sirf color change nahi, balki layout, spacing, responsiveness, and user experience ka main tool hai.
