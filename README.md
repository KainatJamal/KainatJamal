<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=260&color=0:05050A,25:1A0B2E,55:3B0764,80:7C3AED,100:05050A&text=KAINAT%20JAMAL&fontSize=52&fontColor=D4AF37&fontAlignY=42&desc=Computer%20Engineer%20%E2%80%A2%20Full-Stack%20%26%20Mobile%20Developer%20%E2%80%A2%20AI%20Systems&descAlignY=62&descAlign=50&animation=fadeIn"/>

<br/>

<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=600&size=22&duration=2600&pause=900&color=00E5FF&center=true&vCenter=true&width=780&lines=Reverse-Engineering+Wireless+Protocols;Building+Real-Time+Video+%26+Robotics+Systems;Full-Stack+Engineer+%7C+React+%C2%B7+Node+%C2%B7+Flutter;Turning+Ambiguity+Into+Working+Software" />

<br/><br/>

<a href="https://github.com/KainatJamal">
  <img src="https://img.shields.io/badge/GITHUB-05050A?style=for-the-badge&logo=github&logoColor=D4AF37&labelColor=05050A"/>
</a>
<a href="https://www.linkedin.com/in/kainat-jamal-190b73219/">
  <img src="https://img.shields.io/badge/LINKEDIN-05050A?style=for-the-badge&logo=linkedin&logoColor=00E5FF&labelColor=05050A"/>
</a>
<a href="https://www.upwork.com/freelancers/~019966f4eca948ca3e?viewMode=1">
  <img src="https://img.shields.io/badge/UPWORK-05050A?style=for-the-badge&logo=upwork&logoColor=7C3AED&labelColor=05050A"/>
</a>
<a href="mailto:kainat.jamal2@gmail.com">
  <img src="https://img.shields.io/badge/EMAIL-05050A?style=for-the-badge&logo=gmail&logoColor=D4AF37&labelColor=05050A"/>
</a>

</div>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.gif" width="100%"/>

<br/>

## ⟡ &nbsp; About

```yaml
engineer:    Kainat Jamal
title:       Computer Engineer — Full-Stack, AI & Mobile Systems
degree:      BS Computer Engineering — Sir Syed University of Engineering & Technology
status:      Fresh Graduate, 2026
based_in:    Karachi, Pakistan
philosophy:  "If there's no documentation, I read the binary myself."
currently:   Building PakRescue AI — a Flutter/Android control system
             for a WiFi-controlled rescue robot, including a
             clean-room RTP/JPEG video pipeline reverse-engineered
             from a closed-source companion app.
open_to:     Full-Time · Full-Stack · Mobile · AI-Integrated Roles
```

I'm a Computer Engineering graduate who builds working systems end-to-end — from
reverse-engineering an undocumented binary protocol byte-by-byte, to shipping the
polished mobile UI that sits on top of it. My strongest work sits at the intersection
of **low-level systems thinking** (networking, protocols, embedded control) and
**modern product engineering** (React, Node, Flutter, Firebase, LLM integration).

I don't wait for documentation to exist — across my flagship project I used JADX,
Wireshark, and raw packet analysis to reverse-engineer a proprietary TCP/RTP video
protocol with zero source access, then re-implemented it clean-room in Kotlin.

<br/>

## ⟡ &nbsp; Flagship Project

<table>
<tr>
<td width="100%">

### 🛰️ PakRescue AI — Autonomous Rescue Robot Control System

**Flutter · Kotlin · Android Native · Custom RTP/JPEG Video Protocol · WiFi Real-Time Control**

A full control and monitoring application for a custom-built WiFi rescue robot,
built without any vendor SDK, API documentation, or developer support — every
layer of the communication stack was reverse-engineered from scratch.

**What made this hard, and what I did about it:**

- 🔍 **Protocol reverse-engineering** — decompiled the closed-source companion
  APK with JADX, cross-referenced with Wireshark captures, and mapped a
  proprietary binary control protocol over TCP (`CTP:` framed messages —
  topic length, topic, payload length, JSON payload) with zero public spec.
- 📡 **Clean-room video pipeline** — the vendor's video decoder lived inside a
  proprietary native `.so` library. I implemented an independent RFC 2435
  RTP/JPEG reassembler in Kotlin: parsing 12-byte RTP headers, tracking marker
  bits for frame boundaries, and reassembling UDP datagrams into live JPEG frames.
- 🤝 **Handshake sequencing** — reconstructed the exact multi-step session
  negotiation (`APP_ACCESS → VIDEO_PARAM → OPEN_RT_STREAM → keep-alive`)
  required before the robot would even open a video stream.
- 📶 **Unvalidated-WiFi networking** — solved Android's tendency to silently
  drop sockets on internet-less WiFi networks after ~47 seconds by binding
  requests directly to the network via `ConnectivityManager` and a custom
  socket factory — plus a debounced connectivity-loss handler to eliminate a
  flapping reconnect loop caused by network reissuance.
- 🖥️ **Real-time Flutter UI** — a dark-themed live monitoring screen with
  AI-detection overlays, robot controls, and live video rendering, backed by
  native Kotlin platform channels.

**Stack:** `Flutter` `Dart` `Kotlin` `Android SDK` `TCP/UDP Sockets` `RTP/JPEG (RFC 2435)` `JADX` `Wireshark`

</td>
</tr>
</table>

<br/>

## ⟡ &nbsp; Selected Projects

<table>
<tr>
<td width="50%" valign="top">

**🤖 AI-Powered Chatbot**
Full-stack conversational assistant with persistent chat history and topic
management, powered by the Gemini API.
`React` `Node.js` `Express` `MongoDB` `Gemini API`

</td>
<td width="50%" valign="top">

**💬 Real-Time Chat Application**
Instant messaging platform with contact management, media sharing, and
paginated history over WebSockets.
`React` `Node.js` `Socket.IO` `Firebase Firestore` `Firebase Auth`

</td>
</tr>
<tr>
<td width="50%" valign="top">

**📝 Real-Time Collaborative Editor**
Google-Docs-style editor supporting simultaneous multi-user editing, rich text
styling, and `.docx` import/export with version tracking.
`React` `Express.js` `Socket.io` `MongoDB`

</td>
<td width="50%" valign="top">

**🛍️ Kainova — E-Commerce Platform**
Full storefront for apparel and jewelry with cart, checkout, and product
catalog management.
`React` `Django` `HTML/CSS`

</td>
</tr>
<tr>
<td width="50%" valign="top">

**🔐 Secure Authentication System**
Email/password and Google OAuth login with JWT-based session security and a
PostgreSQL-backed user store.
`React` `Node.js` `Express` `PostgreSQL` `JWT` `Firebase`

</td>
<td width="50%" valign="top">

**🏨 Hostel Management System**
End-to-end reservation platform with online booking, payments, and review
workflows for university accommodation.
`PHP` `MySQL` `Bootstrap` `JavaScript`

</td>
</tr>
</table>

<br/>

## ⟡ &nbsp; Engineering Toolkit

<div align="center">

**Languages**

<img src="https://skillicons.dev/icons?i=python,java,cpp,javascript,dart,php&theme=dark"/>

**Mobile & Frontend**

<img src="https://skillicons.dev/icons?i=flutter,kotlin,react,nextjs,html,css,tailwind&theme=dark"/>

**Backend & APIs**

<img src="https://skillicons.dev/icons?i=nodejs,express,fastapi,flask,firebase&theme=dark"/>

**Data & Storage**

<img src="https://skillicons.dev/icons?i=mongodb,mysql,postgres,firebase&theme=dark"/>

**Tooling & Infrastructure**

<img src="https://skillicons.dev/icons?i=git,github,docker,vercel,netlify,postman,wireshark&theme=dark"/>

<br/>

<img src="https://img.shields.io/badge/AI%20%2F%20LLM%20Integration-05050A?style=for-the-badge&logoColor=D4AF37&labelColor=05050A&color=05050A"/>
<img src="https://img.shields.io/badge/Protocol%20Reverse%20Engineering-05050A?style=for-the-badge&labelColor=05050A&color=05050A&logoColor=00E5FF"/>
<img src="https://img.shields.io/badge/Real--Time%20Systems-05050A?style=for-the-badge&labelColor=05050A&color=05050A&logoColor=7C3AED"/>

</div>

<br/>

## ⟡ &nbsp; Experience

<table>
<tr><td width="100%">

**Outreach Automation Specialist** — ManagingSeo *(Internship, Remote)*
`Sep 2025 – Nov 2025`
Built and maintained automated outreach and SEO workflows.

**Operations & Sales Support Associate** — CopyPencil.pk
`Feb 2025 – May 2025`
Tracked 100+ monthly website leads via structured reporting, lifted follow-up
efficiency ~25%, and cut order cancellations ~30% through cross-team
coordination with warehouse and logistics.

**Web Developer** — Gutech International LLC *(Internship, Remote)*
`Nov 2024 – Feb 2025`
Contributed to live production websites, improving UI/UX in an Agile team
environment.

**Full-Stack Web Developer** — Prodigy InfoTech *(Internship, Remote)*
`Nov 2024 – Dec 2024`
Shipped a full authentication system and the Kainova e-commerce platform
end-to-end, from Django backend to React frontend.

**Full-Stack Web Developer** — CodeAlpha *(Internship, Remote)*
`Oct 2024 – Nov 2024`
Delivered a real-time collaborative document editor with Socket.io-based
live sync and version control.

</td></tr>
</table>

<br/>

## ⟡ &nbsp; Freelance

Alongside engineering work, I've delivered **50+ freelance engagements on
Upwork** — 5-star rated — spanning AI-assisted content pipelines, technical
writing, and research-driven documentation for clients across tech and
e-commerce.

<div align="center">
<a href="https://www.upwork.com/freelancers/~019966f4eca948ca3e?viewMode=1">
  <img src="https://img.shields.io/badge/View%20Upwork%20Profile-05050A?style=for-the-badge&logo=upwork&logoColor=7C3AED&labelColor=05050A"/>
</a>
</div>

<br/>

## ⟡ &nbsp; Certifications

<table>
<tr>
<td width="33%" valign="top">

**Cloud & Infrastructure**
- Introduction to Microsoft Azure Cloud Services — *Microsoft*
- Data Storage in Microsoft Azure — *Microsoft*
- Oracle Cloud Infrastructure Foundations — *Oracle*

</td>
<td width="33%" valign="top">

**Software Engineering**
- Version Control — *Meta*
- Programming with JavaScript — *Meta*
- Introduction to Front-End Development — *Meta*

</td>
<td width="33%" valign="top">

**Security & Data**
- Cybersecurity for Everyone — *University of Maryland*
- Introduction to Big Data — *UC San Diego, Rady School*

</td>
</tr>
</table>

<br/>

## ⟡ &nbsp; GitHub Analytics

<div align="center">

<img height="165em" src="https://github-readme-stats.vercel.app/api?username=KainatJamal&show_icons=true&hide_border=true&bg_color=05050A&title_color=D4AF37&icon_color=00E5FF&text_color=E5E5E5&ring_color=7C3AED"/>
<img height="165em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=KainatJamal&layout=compact&hide_border=true&bg_color=05050A&title_color=D4AF37&text_color=E5E5E5&langs_count=8"/>

<br/>

<img src="https://github-readme-streak-stats.herokuapp.com?user=KainatJamal&hide_border=true&background=05050A&stroke=7C3AED&ring=00E5FF&fire=D4AF37&currStreakLabel=D4AF37&sideLabels=E5E5E5&dates=8B8B9E"/>

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=KainatJamal&bg_color=05050A&color=00E5FF&line=7C3AED&point=D4AF37&hide_border=true&area=true"/>

</div>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.gif" width="100%"/>

<div align="center">

<br/>

### Let's build something that hasn't been documented yet.

<a href="mailto:kainat.jamal2@gmail.com"><img src="https://img.shields.io/badge/Email%20Me-05050A?style=for-the-badge&logo=gmail&logoColor=D4AF37&labelColor=05050A"/></a>
<a href="https://www.linkedin.com/in/kainat-jamal-190b73219/"><img src="https://img.shields.io/badge/Connect%20on%20LinkedIn-05050A?style=for-the-badge&logo=linkedin&logoColor=00E5FF&labelColor=05050A"/></a>
<a href="https://www.upwork.com/freelancers/~019966f4eca948ca3e?viewMode=1"><img src="https://img.shields.io/badge/Hire%20Me%20on%20Upwork-05050A?style=for-the-badge&logo=upwork&logoColor=7C3AED&labelColor=05050A"/></a>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=KainatJamal&style=for-the-badge&color=05050A&labelColor=05050A&textColor=D4AF37&label=PROFILE+VIEWS"/>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:05050A,50:3B0764,100:05050A&height=100&section=footer"/>

</div>
