---
theme: default
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## Harnessing Web API Filesystem to Modern Application
  Presentation slides by Kalwabed Rizki @ GDSC UMS, 11 Oct 2023.
drawings:
  persist: false
title: "From OS to Browser: Harnessing Web API Filesystem to Modern Application"
fonts:
  # basically the text
  sans: 'Inter'
  serif: 'Lora'
  # for code blocks, inline code, etc.
  mono: 'Fira Code'
---

<h1 class="text-left !text-5xl p-2">
  From OS to Browser: Harnessing Web API Filesystem to Modern Application
</h1>

<div class="absolute bottom-10 flex flex-col">
  <img src="/gdsc-Logo.png" alt="GDSC logo" width="100" />
  <span>GDSC UMS</span>
  <small>
  Oct 11th, 2023
  </small>
</div>

---
layout: center
class: text-center
---

You can access these slides through

<img src="/gdsc-wf-qrcode.svg" width="300" />

[dub.sh/gdsc-wf](https://dub.sh/gdsc-wf)

---
layout: two-cols
---

<div class="mt-8">
  <h1 class="!text-5xl !pt-8 font-bold">
    Kalwabed Rizki
  </h1>

  <p class="dark:c-gray-400 c-gray-500 !mb10">
    Organizer, JogjaJS
  </p>

- I work as a software engineer at VNT.
- I have a digital garden in <ph-github-logo class="c-gray-500" /> <a href="https://github.com/kalwabed">kalwabed</a>
- For some reason, I get used to putting my moments in <ph-instagram-logo class="c-gray-500" /> <a href="https://www.instagram.com/kalwabed">kalwabed</a>
- and short of my thoughts on <ph-twitter-logo class="c-gray-500" /> <a href="https://twitter.com/kalwabedrzk">kalwabedrzk</a>
    
</div>


::right::

<img src="/kalwabed.jpeg" width="800" alt="My picture" class="rd-full w-52 mt-10 ml-auto ring-4 ring-yellow-500" />

---
layout: statement
---

# Today the browser is almost like an operating system

---
layout: center
class: text-2xl
---

<ul>
  <li>Multi-process architecture</li>
  <li>Extension and Web Apps</li>
  <li>Hardware access</li>
  <li>File system access</li>
  <li>Task management</li>
  <li>User account integration</li>
</ul>

---
layout: center
class: text-sm
---

# Multi-process architecture

<img src="/chrome-task-manager.png" width="700" />

[Image source](https://laptrinhx.com/news/modern-multi-process-browser-architecture-2kwev5P)

---
layout: center
class: text-sm
---

# Extension and web apps

<img src="/chrome-extensions.png" width="700" />

[Image source](https://nektony.com/blog/browser-extensions)

---
layout: center
class: text-sm
---

# Hardware access

<img src="/google-meet.png" width="700" />

---
layout: center
class: text-sm
---

# File system access

<img src="/os-filesys.png" width="500" />

---
layout: center
class: text-sm
---

# Task management

<img src="/chrome-task-manager.webp" width="500" />

---
layout: center
class: text-sm
---

# User account integration

<img src="/add-google-chrome-profile.png" width="250" class="mx-auto" />

[Image source](https://mailmeteor.com/blog/how-to-create-google-chrome-profile)

---
layout: center
class: text-2xl
---

<ul>
  <li class="c-gray2 dark:c-gray6">Multi-process architecture</li>
  <li class="c-gray2 dark:c-gray6">Extension and Web Apps</li>
  <li class="c-gray2 dark:c-gray6">Hardware access</li>
  <li class="c-blue">File system access</li>
  <li class="c-gray2 dark:c-gray6">Task management</li>
  <li class="c-gray2 dark:c-gray6">User account integration</li>
</ul>

---
layout: section
---

# File System Access
How do the operating system and browser manage this thing?

---
layout: center
---

# File System Access in the Operating System

<img src="/filesystem-dark.svg" width="500" class="mx-auto hidden dark:block" />
<img src="/filesystem.svg" width="500" class="mx-auto dark:hidden" />

---
layout: two-cols
class: items-center
---

# File System Access in the Operating System
Provides greater flexibility to users.

- File permissions
- Access control lists (ACLs)
- Security policies
- Logging and auditing
- Network file system

::right::

<img src="/filesystem-dark.svg" width="500" class="mx-auto hidden dark:block" />
<img src="/filesystem.svg" width="500" class="mx-auto dark:hidden" />

---
layout: statement
---

# What if we pull this system into the browser domain?

---
layout: center
---

It can be implemented, but currently with limitations (unfortunately):
1. Control
    - full control over the file system.
2. Isolation
    - strong isolation between processes and users.
3. Security
    - relies on same-origin policy and user consent.
4. Permissions 
    - manages user and group permissions.
5. Use cases 
    - interact with files and data within the context of a web page.

---
layout: section
---

# So What's Web Filesystem API?

---
layout: center
---

# Web Filesystem API
The term "Web API Filesystem" typically refers to the Filesystem Access API.

This API is a part of the broader web platform and allows web applications to interact with the user's local file system from within a web browser.

It provides a set of methods and features for reading, writing, creating, and deleting files and directories.

---
layout: statement
---

# What solution does the Web API Filesystem bring?

---
layout: center
---

# Web API Filesystem solutions
1. Access to local files
2. Offline web apps (PWA)
3. Data persistence
4. Document editing
5. Development flexibility

---
layout: statement
---

# What about browser support?
Of course, we also have to pay attention to browser support when talking about Web APIs.

---
layout: center
---

<img src="/browser-support-1.png" width="450" height="400" alt="Browser support 1" />

source: MDN

---
layout: center
---

`FileSystemWritableFileStream`
<img src="/browser-support-2.png" width="450" height="400" alt="Browser support 2" />

source: MDN

---
layout: center
---

# Web API Filesystem shortcomings
- Limited browser support
- Storage quotas
- Complexity
- Lack of native integration

---
layout: center
---

# Recap
- OS manages files, permissions, and security.
- Extend OS-like file access to web apps.
- Web Filesystem API enables browser file access.
- Solutions: Offline apps, document editing, data storage.
- Shortcomings: Browser limits, storage quotas, complexity.
- Priorities: User clarity, privacy, security.

---
layout: end
---

Thank you!

Slides can be found on [kalwabed.xyz/talks](https://www.kalwabed.xyz/talks)
