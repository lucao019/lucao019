<div align="center">

<!-- HEADER ANIMADO -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:111827,100:1a1a2e&height=200&section=header&text=lucao019&fontSize=55&fontColor=ffffff&animation=twinkling&fontAlignY=38&desc=Software%20%E2%80%A2%20Hardware%20%E2%80%A2%20Automation%20%E2%80%A2%20System%20Optimization&descAlignY=60&descSize=15&descColor=a78bfa"/>

<!-- TYPING ANIMATION -->
<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=16&pause=1000&color=a78bfa&center=true&width=500&lines=JavaScript+%7C+TypeScript+%7C+Node.js+%7C+Python;React+%7C+Vite+%7C+Next.js+%7C+Express;Discord+Bots+%7C+OBS+Overlays+%7C+CLI+Tools;Build+%E2%86%92+Test+%E2%86%92+Measure+%E2%86%92+Refine" alt="Typing SVG"/>
</a>

<br/>

<!-- BADGES -->
<img src="https://komarev.com/ghpvc/?username=lucao019&style=for-the-badge&color=7c3aed&label=PROFILE+VIEWS" alt="Profile Views"/>
&nbsp;
<img src="https://img.shields.io/badge/Focus-Practical%20Engineering-7c3aed?style=for-the-badge&labelColor=0d1117" alt="Focus"/>
&nbsp;
<img src="https://img.shields.io/badge/Status-Always%20Building-f59e0b?style=for-the-badge&labelColor=0d1117" alt="Status"/>

</div>

---

## 🎮 Open Source Contribution — Bloodborne PC (Windows Port)

<div align="center">

<a href="https://github.com/lucao019/bloodborne_pc_windows_port">
  <img src="https://img.shields.io/badge/bloodborne__pc__windows__port-0d1117?style=for-the-badge&logo=github&logoColor=a78bfa&labelColor=0d1117" alt="bloodborne_pc_windows_port"/>
  <img src="https://img.shields.io/badge/TYPE-C%2B%2B%20%7C%20CMake%20%7C%20Build%20Systems-f59e0b?style=for-the-badge&labelColor=0d1117" alt="type"/>
  <img src="https://img.shields.io/badge/PLATFORM-Windows%2011%20%7C%20MSYS2%20UCRT64-a78bfa?style=for-the-badge&labelColor=0d1117" alt="platform"/>
</a>

<br/><br/>

<sub>
Fork of <a href="https://github.com/Mrsuss60/bloodborne_pc_windows_port">Mrsuss60/bloodborne_pc_windows_port</a> —
native Windows build fixes that were missing from the original repository
</sub>

</div>

<br/>

> The original project **did not compile on Windows**. Three independent failures blocked any build attempt. I diagnosed each one, applied the fixes and documented the full process.

<br/>

<table>
<tr>
<td width="40px" align="center">📦</td>
<td><strong>miniz — silent CMake failure</strong><br/>
The original <code>CMakeLists.txt</code> tried to locate miniz via <code>find_path</code> pointing at MSYS2/MinGW64. No MSYS2 package installs it there, so CMake silently resolved <code>MINIZ_INC=NOTFOUND</code> and linking failed. Replaced the broken lookup with <code>add_subdirectory</code> over the upstream source, making it self-contained with no system package required.</td>
</tr>
<tr>
<td width="40px" align="center">⚙️</td>
<td><strong>xbyak — invisible missing dependency</strong><br/>
The embedded shadPS4 shader recompiler uses xbyak for runtime x86-64 code generation. The original repo had <strong>no xbyak reference anywhere</strong> — no submodule, no CMake entry, nothing. Any Windows build attempt ended immediately with <code>fatal error: xbyak/xbyak.h: No such file or directory</code>. Added herumi/xbyak as a submodule and wired it into CMake.</td>
</tr>
<tr>
<td width="40px" align="center">🔗</td>
<td><strong>LTO — linker crash at the final step</strong><br/>
With link-time optimization enabled globally, GCC's LTO pass discarded functions only referenced from inline assembly strings (<code>call pre_import_hook</code>, <code>call restore_guest_fs</code>), causing <code>undefined reference</code> errors at the very last link step — after everything else compiled successfully. Identified the interaction between <code>__attribute__((sysv_abi))</code> + <code>asm volatile</code> and LTO on Windows/MinGW. Disabled LTO selectively on the <code>bbport</code> target, preserving it for <code>bbgpu</code>.</td>
</tr>
<tr>
<td width="40px" align="center">📄</td>
<td><strong>Full porting documentation</strong><br/>
Wrote a <a href="https://github.com/lucao019/bloodborne_pc_windows_port/blob/master/WINDOWS_BUILD_PORTING_LOG.md">807-line technical log</a> covering the complete build environment, all required MSYS2 packages, each error with root cause and fix, and a step-by-step reproduction guide for a clean Windows install.</td>
</tr>
</table>

---

## 🧠 system.profile

```typescript
const lucao019 = {
  focus:        "Practical software projects and PC/system optimization",
  languages:    ["JavaScript", "TypeScript", "Python", "PowerShell", "C", "C++"],
  web:          ["HTML", "CSS", "React", "Vite", "Next.js"],
  backend:      ["Node.js", "Express", "REST APIs", "SQLite"],
  integrations: ["Discord Bots", "OBS Overlays", "Local-network Tools"],
  tools:        ["Git", "Windows", "FFmpeg", "CLI Workflows", "CMake", "GCC", "MSYS2"],
  method:       "prototype -> test -> measure -> refine",
  status:       "always building 🚀",
};
```

---

<div align="center">

## ⚡ Tech Stack

<br/>

**Languages**

<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=js,ts,python,powershell&perline=6"/>
</a>

<br/><br/>

**Frontend**

<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=html,css,react,vite,nextjs&perline=6"/>
</a>

<br/><br/>

**Backend & Data**

<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=nodejs,express,sqlite&perline=6"/>
</a>

<br/><br/>

**Tools**

<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=git,github,vscode,discord,linux&perline=6"/>
</a>

</div>

---

<div align="center">

## 📊 GitHub Stats

<br/>

<img height="195" src="https://github-readme-stats.vercel.app/api?username=lucao019&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=0d1117&title_color=a78bfa&icon_color=f59e0b&text_color=c9d1d9&ring_color=7c3aed" alt="GitHub Stats"/>
&nbsp;
<img height="195" src="https://github-readme-stats.vercel.app/api/top-langs/?username=lucao019&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=a78bfa&text_color=c9d1d9&langs_count=8" alt="Top Langs"/>

<br/><br/>

<img width="60%" src="https://streak-stats.demolab.com/?user=lucao019&theme=tokyonight&hide_border=true&background=0d1117&ring=a78bfa&fire=f59e0b&currStreakLabel=a78bfa&sideLabels=c9d1d9&currStreakNum=ffffff&sideNums=ffffff&dates=8b949e" alt="GitHub Streak"/>

<br/><br/>

<img width="95%" src="https://github-readme-activity-graph.vercel.app/graph?username=lucao019&bg_color=0d1117&color=a78bfa&line=7c3aed&point=f59e0b&area=true&area_color=7c3aed&hide_border=true&custom_title=lucao019's%20Contribution%20Graph" alt="Activity Graph"/>

</div>

---

## 🔥 Projects

<div align="center">

<!-- PUBG STATS -->
<a href="https://github.com/lucao019/PUBG-STATS">
  <img src="https://img.shields.io/badge/PUBG--STATS-0d1117?style=for-the-badge&logo=github&logoColor=a78bfa&labelColor=0d1117" alt="PUBG-STATS"/>
  <img src="https://img.shields.io/badge/TYPE-OBS%20Overlay-f59e0b?style=for-the-badge&labelColor=0d1117" alt="type"/>
  <img src="https://img.shields.io/badge/STACK-Node.js%20%7C%20Express-a78bfa?style=for-the-badge&labelColor=0d1117" alt="stack"/>
</a>

<br/>
<sub>Local PUBG statistics overlay for OBS — kills, damage, matches, weapon performance</sub>

<br/><br/>

<!-- CHECKIN BOT -->
<a href="https://github.com/lucao019/discord-checkin-bot">
  <img src="https://img.shields.io/badge/CheckIn%20Bot-0d1117?style=for-the-badge&logo=discord&logoColor=a78bfa&labelColor=0d1117" alt="CheckIn Bot"/>
  <img src="https://img.shields.io/badge/TYPE-Discord%20Bot-f59e0b?style=for-the-badge&labelColor=0d1117" alt="type"/>
  <img src="https://img.shields.io/badge/STACK-TypeScript%20%7C%20discord.js-a78bfa?style=for-the-badge&labelColor=0d1117" alt="stack"/>
</a>

<br/>
<sub>Detects new members and creates profile cards with account, server and profile details</sub>

<br/><br/>

<!-- LUCAO LINK -->
<a href="https://github.com/lucao019/cam-audio-to-windows">
  <img src="https://img.shields.io/badge/LUCAO%20LINK-0d1117?style=for-the-badge&logo=android&logoColor=a78bfa&labelColor=0d1117" alt="LUCAO LINK"/>
  <img src="https://img.shields.io/badge/TYPE-Android%20→%20PC%20Stream-f59e0b?style=for-the-badge&labelColor=0d1117" alt="type"/>
  <img src="https://img.shields.io/badge/STACK-Node.js%20%7C%20FFmpeg%20%7C%20TCP-a78bfa?style=for-the-badge&labelColor=0d1117" alt="stack"/>
</a>

<br/>
<sub>Phone camera stream to PC over local network — H.264 video tested, mic streaming in development</sub>

</div>

---

<!-- FOOTER ANIMADO -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,50:111827,100:0f0c29&height=120&section=footer&animation=twinkling"/>
