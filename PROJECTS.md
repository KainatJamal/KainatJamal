<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:6D28D9,100:0D1117&height=180&section=header&text=PROJECTS&fontSize=40&fontColor=F5F3FF&fontAlignY=42&animation=fadeIn" width="100%"/>

<a href="./EXPERIENCE.md"><img src="https://img.shields.io/badge/←_EXPERIENCE-0D1117?style=for-the-badge&color=8B5CF6"/></a>
<a href="./README.md"><img src="https://img.shields.io/badge/HOME-0D1117?style=for-the-badge&color=D4AF37"/></a>
<a href="./SKILLS.md"><img src="https://img.shields.io/badge/SKILLS_→-0D1117?style=for-the-badge&color=22D3EE"/></a>

</div>

<br/>

## 🏆 Flagship Project

### PakRescue AI

<img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white"/>
<img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white"/>
<img src="https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white"/>
<img src="https://img.shields.io/badge/JADX-8B5CF6?style=flat-square"/>
<img src="https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white"/>
<img src="https://img.shields.io/badge/TCP%2FUDP-22D3EE?style=flat-square"/>
<img src="https://img.shields.io/badge/RTP%20%2F%20RFC%202435-8B5CF6?style=flat-square"/>

**An Android app that pilots and monitors a WiFi-connected rescue robot in real time — built without any official protocol documentation.**

**The problem:** the rescue car ships with a closed-source companion APK. No public docs, no API reference — just a working app and a WiFi hotspot.

**The approach:**
- Decompiled the manufacturer's APK with **JADX** to study its networking and media-playback internals
- Captured live traffic in **Wireshark** to map the actual wire protocol against the decompiled source
- Reverse-engineered a custom **TCP control channel** (a length-prefixed JSON framing protocol) used for commands like connect, start-stream, and stop-stream
- Rebuilt the **live video pipeline** by hand: an RTP-over-UDP transport carrying RFC 2435 JPEG-over-RTP frames, reassembled fragment-by-fragment using RTP timestamps and marker bits
- Solved an Android-specific networking bug where the OS silently drops an "unvalidated" WiFi connection (no internet access) from the routing table after ~47 seconds, by binding sockets directly to the WiFi network interface

**Stack:** Flutter (UI) + native Kotlin (networking, media, platform channels)

**Status:** Final Year Project (FYP), in active development

<sub>Private repository — case study and code available on request.</sub>

<br/>

---

<br/>

## 💻 Other Builds

<table>
<tr>
<td width="50%" valign="top">

**🤖 AI-Powered Chatbot**
A conversational AI assistant with chat history and topic management, powered by the Google Gemini API.

`React.js` `Node.js` `Express` `MongoDB` `Gemini API`

<a href="https://github.com/KainatJamal/AI-Powered-Chatbot">↳ Repository</a>

</td>
<td width="50%" valign="top">

**🛍️ Kainova — E-Commerce Website**
A shopping platform for apparel and jewelry with product listings, cart, and checkout flow.

`React.js` `Django` `HTML` `CSS`

<a href="https://github.com/KainatJamal/Kainova---An-E-commerce-Website">↳ Repository</a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

**💬 Real-Time Chat App**
Instant messaging with contact management, media sharing, and search — built on Socket.IO and Firebase.

`React.js` `Node.js` `Express` `Socket.IO` `Firebase`

<a href="https://github.com/KainatJamal/Real-Time-Chat-App">↳ Repository</a>

</td>
<td width="50%" valign="top">

**📝 Real-Time Collaborative Editor**
Google-Docs-style multi-user document editor with live sync, text styling, and `.docx` import/export.

`React` `Express.js` `Socket.io` `MongoDB`

<a href="https://github.com/KainatJamal/Collaborative-Editor">↳ Repository</a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

**📱 Social Media Platform**
Post creation, likes, trending hashtags, and JWT-secured auth with profile image uploads.

`React.js` `Node.js` `Express` `MongoDB` `JWT`

<a href="https://github.com/KainatJamal/Social-Media-Website">↳ Repository</a>

</td>
<td width="50%" valign="top">

**🔐 User Authentication System**
Secure login/signup with email-password and Google auth, backed by JWT and Firebase.

`React` `Node.js` `Express` `PostgreSQL` `Firebase` `JWT`

<a href="https://github.com/KainatJamal/Login-Sigup-Form">↳ Repository</a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

**🏢 SSUET Hostel Management System**
A hostel booking platform with student registration, room reservations, and payment options.

`PHP` `MySQL` `Bootstrap` `JavaScript`

</td>
<td width="50%" valign="top">

</td>
</tr>
</table>

<br/>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:6D28D9,100:0D1117&height=100&section=footer"/>

<a href="./EXPERIENCE.md"><img src="https://img.shields.io/badge/←_EXPERIENCE-0D1117?style=for-the-badge&color=8B5CF6"/></a>
<a href="./README.md"><img src="https://img.shields.io/badge/HOME-0D1117?style=for-the-badge&color=D4AF37"/></a>
<a href="./SKILLS.md"><img src="https://img.shields.io/badge/SKILLS_→-0D1117?style=for-the-badge&color=22D3EE"/></a>

</div>
