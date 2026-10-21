<p align="center">
  <img src="./assets/profile-banner-night.gif" alt="Langit malam pixel-art dengan sosok berjubah dan kota bercahaya" width="100%" />
</p>

<h1 align="center">Akbar</h1>

<p align="center">
  <strong>Roblox Luau UI Developer · Web App Developer</strong><br />
  Membangun pustaka antarmuka Roblox dan aplikasi web full-stack yang rapi, cepat, dan enak dipakai.
</p>

<p align="center">
  <a href="https://github.com/Akbar025zzz/kingAkbarUi-Speedhub"><img src="https://img.shields.io/badge/Luau-00A2FF?style=for-the-badge&logo=roblox&logoColor=white" alt="Luau" /></a>
  <a href="https://www.lua.org/"><img src="https://img.shields.io/badge/Lua-2C2D72?style=for-the-badge&logo=lua&logoColor=white" alt="Lua" /></a>
  <a href="https://www.typescriptlang.org/"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" /></a>
  <a href="https://nextjs.org/"><img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" /></a>
  <a href="https://nodejs.org/"><img src="https://img.shields.io/badge/Node.js-5FA04E?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js" /></a>
  <a href="https://www.postgresql.org/"><img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" /></a>
  <a href="https://tailwindcss.com/"><img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" /></a>
  <a href="https://www.docker.com/"><img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" /></a>
</p>

## Tentang

Saya mengerjakan dua hal yang saling melengkapi: antarmuka di dalam Roblox dengan Luau, dan aplikasi web dengan Next.js serta Node.js. Fokus saya ada di hal yang sering dilewatkan orang lain, yaitu komponen yang perilakunya konsisten, dokumentasi yang bisa langsung dipakai, dan kode yang tetap enak dirawat setelah proyeknya membesar.

Dua proyek di bawah ini saya bangun dari nol, lengkap dengan dokumentasi penggunaan, contoh kode, dan catatan arsitekturnya.

## Proyek pilihan

### [KingAkbarUI Speedhub](https://github.com/Akbar025zzz/kingAkbarUi-Speedhub) — pustaka UI Roblox

Pustaka antarmuka Luau bergaya gelap modern untuk script hub dan tool, nyaman dipakai di PC maupun HP. Versi 1.7 menyertakan 11 komponen siap pakai: Button, Toggle, Slider, Input, Dropdown, Keybind, ColorPicker, Panel, Paragraph, Seperator, dan Line, ditambah kotak pengelompok Section, GroupBox, serta TabBox.

Window-nya menyesuaikan ukuran layar, bisa digeser, dan punya tombol floating serta hotkey untuk tampil atau sembunyi. Tersedia notifikasi, badge topbar, pencarian tab, profil pemain, serta tema dan font yang bisa diganti. Setiap komponen menerima dua gaya penulisan, jadi bisa dipilih sesuai selera, dan pustaka ini aman dijalankan berulang kali karena UI lama dibersihkan otomatis.

```lua
local Lib = loadstring(game:HttpGet(
  "https://raw.githubusercontent.com/Akbar025zzz/kingAkbarUi-Speedhub/refs/heads/main/init.lua"
))()

local Win = Lib:CreateWindow({ "King Akbar", "v1.7", 100, UDim2.fromOffset(420, 280) })
local Tab = Win:CreateTab({ "Main", "rbxassetid://7734010488" })
local Sec = Tab:AddSection("Farm", true)

Sec:AddToggle({ "Auto Farm", "Farm otomatis", false, function(v) print("Farm:", v) end })
Sec:AddSlider({ "WalkSpeed", "", 1, 16, 200, 16, function(v) print("Speed:", v) end })

Lib:SetNotification({ "King Akbar", "Loaded", "Script berhasil dimuat" })
```

<p>
  <a href="https://github.com/Akbar025zzz/kingAkbarUi-Speedhub"><img src="https://img.shields.io/badge/Lihat%20repositori-181717?style=for-the-badge&logo=github&logoColor=white" alt="Lihat repositori KingAkbarUI Speedhub" /></a>
  <img src="https://img.shields.io/badge/versi-1.7-00A2FF?style=for-the-badge" alt="Versi 1.7" />
  <img src="https://img.shields.io/badge/lisensi-MIT-3DA639?style=for-the-badge" alt="Lisensi MIT" />
  <img src="https://img.shields.io/badge/dokumentasi-lengkap-8A2BE2?style=for-the-badge" alt="Dokumentasi lengkap" />
</p>

### [Nobar King Akbar Anime](https://github.com/Akbar025zzz/nobar-king-akbar-anime) — streaming anime dan nonton bareng

Aplikasi web untuk katalog anime sub Indo dan menonton bareng secara realtime. Host mengendalikan pemutaran, semua peserta mengikuti dengan toleransi selisih 1,6 detik, dan obrolan room berjalan langsung dengan riwayat 100 pesan terakhir.

<p align="center">
  <a href="https://github.com/Akbar025zzz/nobar-king-akbar-anime">
    <img src="https://raw.githubusercontent.com/Akbar025zzz/nobar-king-akbar-anime/main/docs/screenshots/01-home.png" alt="Beranda Nobar King Akbar Anime dengan room yang sedang berjalan" width="100%" />
  </a>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/Akbar025zzz/nobar-king-akbar-anime/main/docs/screenshots/19-room-play-host.png" alt="Room nobar dengan pemutaran tersinkron, daftar peserta, dan obrolan" width="49%" />
  <img src="https://raw.githubusercontent.com/Akbar025zzz/nobar-king-akbar-anime/main/docs/screenshots/23-film-detail.png" alt="Halaman detail film dengan metadata TMDb dan daftar pemain" width="49%" />
</p>

Selain anime, ada seksi Film dan Series yang mengambil metadata langsung dari TMDb dalam bahasa Indonesia: Film Indonesia, film populer, drakor, dan dracin, lengkap dengan pemilih musim, daftar episode, dan trailer. Pemutarnya memilih server tercepat lewat rantai resolver, memutar HLS dengan hls.js, dan memulihkan error otomatis. Pengguna memiliki akun dengan sesi cookie HttpOnly, token yang di-hash, rate limit anti brute-force, favorit, serta riwayat tontonan yang bisa dilanjutkan dari profil. Seluruh antarmuka berbahasa Indonesia, responsif di ponsel, dan dibungkus Docker.

<p>
  <a href="https://github.com/Akbar025zzz/nobar-king-akbar-anime"><img src="https://img.shields.io/badge/Lihat%20repositori-181717?style=for-the-badge&logo=github&logoColor=white" alt="Lihat repositori Nobar King Akbar Anime" /></a>
  <img src="https://img.shields.io/badge/Next.js_15-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js 15" />
  <img src="https://img.shields.io/badge/React_19-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React 19" />
  <img src="https://img.shields.io/badge/Socket.IO_4-010101?style=for-the-badge&logo=socketdotio&logoColor=white" alt="Socket.IO 4" />
  <img src="https://img.shields.io/badge/PostgreSQL_16-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL 16" />
</p>

## Aktivitas GitHub

<p align="center">
  <a href="https://github.com/Akbar025zzz">
    <img src="./github-metrics.svg" alt="Ringkasan statistik dan aktivitas GitHub Akbar" width="480" />
  </a>
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Akbar025zzz&layout=compact&langs_count=8&theme=tokyonight" alt="Bahasa pemrograman yang paling sering digunakan Akbar" width="480" />
</p>

<p align="center"><sub>Kartu bahasa oleh <a href="https://github.com/anuraghazra/github-readme-stats">github-readme-stats</a>.</sub></p>

<p align="center">
  <a href="https://github.com/Akbar025zzz">
    <img src="./metrics.calendar.svg" alt="Kalender kontribusi GitHub Akbar" width="100%" />
  </a>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Akbar025zzz/Akbar025zzz/output/github-contribution-grid-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Akbar025zzz/Akbar025zzz/output/github-contribution-grid-snake.svg" />
    <img src="https://raw.githubusercontent.com/Akbar025zzz/Akbar025zzz/output/github-contribution-grid-snake.svg" alt="Animasi ular bergerak di kalender kontribusi GitHub" width="100%" />
  </picture>
</p>

---

<p align="center">
  <a href="https://github.com/Akbar025zzz?tab=repositories">Semua repositori</a>
</p>
