<div align="center">

# ⚡ CODERVISUAL DEVELOPER TOOLKIT

### 🚀 Full Stack Developer | System Engineer | DevOps Explorer

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,100:2c5364&height=220&section=header&text=Developer%20Command%20Hub&fontSize=32&fontColor=ffffff" />

---

## 💡 About This Repository

🧠 A complete **Developer Command Hub** for Windows, Laravel, Git, Node.js & System Tools  

⚙️ Beginner → Intermediate → Advanced all-in-one guide  

🚀 Safe, Legal & Production-ready commands only  

---

## ⚡ Tech Stack Covered

<div align="center">

![Windows](https://img.shields.io/badge/Windows-System-blue)
![Laravel](https://img.shields.io/badge/Laravel-Framework-red)
![Git](https://img.shields.io/badge/Git-VersionControl-orange)
![Node.js](https://img.shields.io/badge/Node.js-JS-green)
![PowerShell](https://img.shields.io/badge/PowerShell-Automation-blue)
![MySQL](https://img.shields.io/badge/MySQL-Database-lightblue)

</div>

---

## 🚀 Quick Start

```bash
git clone https://github.com/codexvisual/your-repo-name
cd your-repo-name
```

---

# 🧑‍💻 CORE COMMAND MODULES

---

## 🖥 WINDOWS COMMANDS

⚡ System Info  
```powershell
systeminfo
winver
```

🧹 Cleanup & Speed  
```powershell
cleanmgr
del /q/f/s %TEMP%\*
taskmgr
```

🌐 Network Tools  
```powershell
ipconfig
ipconfig /flushdns
ping google.com
```

🔐 Security  
```powershell
windowsdefender:
Start-MpScan -ScanType QuickScan
```

---

## ⚙️ LARAVEL COMMANDS

🚀 Setup  
```bash
composer create-project laravel/laravel app
php artisan serve

<img src="https://github-readme-streak-stats.herokuapp.com/?user=codexvisual&theme=tokyonight" />

---

## ⚠ Disclaimer

This repository is for **educational & development purposes only**.  
All commands are safe, legal & system-approved tools.

---

## 🤝 Connect

[![GitHub](https://img.shields.io/badge/GitHub-codexvisual-black)](https://github.com/codexvisual)
[![Email](https://img.shields.io/badge/Email-Contact-red)](mailto:rahat830611@gmail.com)

---

## ⚡ Quote

> “Clean code, smart system, scalable future.”

---

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,100:0f2027&height=120&section=footer" />

</div>
# 🚀 Laravel Commands Key Guide (What does what?)

A simple explanation guide for Laravel + PHP + Composer commands.

---

# 🧱 1. PHP & Composer (Base Setup)

## 🔑 php -v
👉 PHP version check করে  
✔ Use: জানতে PHP install আছে কিনা

## 🔑 composer -V
👉 Composer version check  
✔ Use: Laravel dependency manager working কিনা check

## 🔑 composer install
👉 Project এর সব packages install করে  
✔ Use: নতুন project clone করার পর

## 🔑 composer update
👉 Packages latest version এ update করে  
✔ Use: dependency refresh করার জন্য

---

# 🚀 2. Laravel Project Setup

## 🔑 composer create-project laravel/laravel app
👉 নতুন Laravel project তৈরি করে  
✔ Use: fresh project start করার জন্য

## 🔑 php artisan serve
👉 Local server run করে  
✔ Use: http://127.0.0.1:8000 চালাতে

---

# 🔑 3. App Key & Config

## 🔑 php artisan key:generate
👉 Security key generate করে (.env file এ)  
✔ Use: project first setup

## 🔑 php artisan config:clear
👉 Config cache clear করে  
✔ Use: .env change করলে

## 🔑 php artisan config:cache
👉 Config cache করে performance boost দেয়  
✔ Use: production server

---

# 🗄 4. Database (Migration System)

## 🔑 php artisan migrate
👉 Database table create করে  
✔ Use: DB structure apply করতে

## 🔑 php artisan migrate:fresh
👉 সব table delete করে নতুন করে তৈরি করে  
✔ Use: clean reset database

## 🔑 php artisan migrate:rollback
👉 last migration undo করে  
✔ Use: mistake fix করতে

## 🔑 php artisan migrate:reset
👉 সব migration rollback করে  
✔ Use: full reset

---

# 🧱 5. MVC (Model - View - Controller)

## 🔑 php artisan make:model Product
👉 Model তৈরি করে  
✔ Use: database table represent করতে

## 🔑 php artisan make:model Product -m
👉 Model + Migration একসাথে তৈরি  
✔ Use: database ready structure

## 🔑 php artisan make:model Product -mc
👉 Model + Migration + Controller তৈরি  
✔ Use: full feature setup

---

## 🔑 php artisan make:controller ProductController
👉 Controller তৈরি করে  
✔ Use: logic handle করতে

## 🔑 php artisan make:controller ProductController -r
👉 Resource Controller (CRUD ready)  
✔ Use: full CRUD system

---

## 📄 View (Blade)

👉 View file manually তৈরি করতে হয়:

```
resources/views/home.blade.php
```

✔ Use: UI design show করার জন্য

---

# 🌐 6. Routes (URL System)

## 🔑 Route Example
```php
Route::get('/', function () {
    return view('welcome');
});
```

👉 কাজ: URL কে page/logic এর সাথে connect করে

## 🔑 Controller Route
```php
Route::get('/products', [ProductController::class, 'index']);
```

✔ Use: controller call করার জন্য

---

# 🧪 7. Tinker (Testing Tool)

## 🔑 php artisan tinker
👉 Live database test tool  
✔ Use: query test without UI

Example:
```php
App\Models\User::all();
```

---

# ⚡ 8. Cache & Performance

## 🔑 php artisan optimize:clear
👉 সব cache clear করে  
✔ Use: error fix / update apply

## 🔑 php artisan optimize
👉 system optimize করে speed boost  
✔ Use: production

## 🔑 php artisan route:cache
👉 routes cache করে speed বাড়ায়  
✔ Use: live server

---

# 🧵 9. Queue System

## 🔑 php artisan queue:work
👉 background job চালায়  
✔ Use: email / task processing

## 🔑 php artisan queue:restart
👉 queue restart করে  
✔ Use: updates apply

---

# 🧰 10. Maintenance Mode

## 🔑 php artisan down
👉 site বন্ধ করে maintenance mode  
✔ Use: update time

## 🔑 php artisan up
👉 site আবার live করে  
✔ Use: maintenance শেষ

---

# 📦 11. Seeder & Factory

## 🔑 php artisan make:seeder UserSeeder
👉 dummy data insert tool  
✔ Use: testing data

## 🔑 php artisan db:seed
👉 seeder run করে  
✔ Use: database fill

## 🔑 php artisan make:factory ProductFactory
👉 fake data generator  
✔ Use: testing system

---

# 🔐 12. Authentication (Login System)

## 🔑 laravel/ui install
```bash
composer require laravel/ui
php artisan ui bootstrap --auth
npm install
npm run dev
```

✔ Use: login/register system

---

# 📊 13. Important Debug Commands

## 🔑 php artisan route:list
👉 সব routes দেখায়  
✔ Use: debugging URL

## 🔑 php artisan --version
👉 Laravel version check  
✔ Use: info check

---

# 💡 FINAL SUMMARY

✔ Model = Database structure  
✔ View = UI design  
✔ Controller = Logic  
✔ Migration = Database setup  
✔ Route = URL system  
✔ Tinker = Live testing tool  

---

# ⚠ Note

সব commands Laravel official system based & safe for development use.

---

Made with ❤️ by CodexVisual
