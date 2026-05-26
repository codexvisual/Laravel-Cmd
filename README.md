<div align="center">

# 🚀 Ultimate Laravel Commands Key Guide

**PHP · Composer · Artisan · Terminal**  
_The only cheat sheet you'll ever need_

[![Made with Love](https://img.shields.io/badge/Made%20with-Love-FF2D20?style=for-the-badge&logo=laravel)](https://laravel.com)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=for-the-badge)](https://github.com/your-username/your-repo/pulls)

</div>

---

## 🧱 1. PHP & Composer (Base Setup)

<div align="center">

| 💻 Command | 📖 What it does |
|:-----------|:----------------|
| `php -v` | PHP version check — নিশ্চিত করুন সব ঠিক আছে |
| `composer -V` | Composer version check |
| `composer install` | `composer.lock` অনুযায়ী প্যাকেজ ইনস্টল |
| `composer update` | `composer.json` অনুযায়ী সব আপডেট |

</div>

---

## 🚀 2. Laravel Project Setup

<div align="center">

| Command | Description |
|:--------|:------------|
| `composer create-project laravel/laravel project-name` | একদম নতুন প্রজেক্ট তৈরি |
| `php artisan serve` | লোকাল সার্ভার রান (http://127.0.0.1:8000) |

</div>

---

## 🔑 3. App Key & Configuration

<div align="center">

| Command | Description |
|:--------|:------------|
| `php artisan key:generate` | `.env`-এ সিকিউর কী জেনারেট |
| `php artisan config:clear` | কনফিগ ক্যাশ ক্লিয়ার — পরিবর্তন তাৎক্ষণিক এপ্লাই |
| `php artisan config:cache` | **Production**-এ কনফিগ ক্যাশ করে পারফরম্যান্স বাড়ান |

</div>

---

## 🗄 4. Database & Migration System

<div align="center">

| Command | Description |
|:--------|:------------|
| `php artisan migrate` | সব পেন্ডিং মাইগ্রেশন রান |
| `php artisan migrate:rollback` | শেষ ব্যাচ রোলব্যাক (`--step=5`) |
| `php artisan migrate:fresh` | ডাটাবেজ ড্রপ + স্ক্র্যাচ থেকে মাইগ্রেট |
| `php artisan migrate:refresh` | রোলব্যাক + রান (ড্রপ ছাড়া) |
| `php artisan migrate:status` | মাইগ্রেশন স্ট্যাটাস টেবিল |

</div>

---

## 🧱 5. MVC & Core Component Generation (`make`)

<div align="center">

| ⚡ Command | 🎯 Creates |
|:-----------|:-----------|
| `php artisan make:model Product` | Only Model |
| `php artisan make:model Product -m` | Model + Migration |
| `php artisan make:model Product -mc` | Model + Migration + Controller |
| `php artisan make:model Product -mrcs` | All-in-one: Model, Migration, Resource Controller, Factory, Seeder |
| `php artisan make:controller ProductController` | Plain Controller |
| `php artisan make:controller ProductController -r` | Resource Controller (CRUD) |
| `php artisan make:controller ProductController --api` | API Controller (RESTful) |
| `php artisan make:middleware CheckAdmin` | Middleware filter |
| `php artisan make:request StoreProductRequest` | Form Request (Validation) |

</div>

---

## 📂 6. File System & Views (Terminal Basics)

<div align="center">

| 🖥️ Command | 📁 Action |
|:------------|:----------|
| `cd resources/views` | Views ফোল্ডারে যান |
| `cd ..` | প্যারেন্ট ডিরেক্টরিতে ফিরুন |
| `ls` (Linux/macOS) / `dir` (Windows) | ফাইল-ফোল্ডার তালিকা |
| `mkdir admin` | নতুন ফোল্ডার তৈরি |
| `touch home.blade.php` (Linux/macOS) | নতুন Blade ফাইল |
| `type nul > home.blade.php` (Windows) | নতুন Blade ফাইল |

</div>

---

## ✨ Bonus: Quick Artisan Reference

```bash
# Clear everything
php artisan optimize:clear

# Tinker playground
php artisan tinker

# List all routes
php artisan route:list

# Create symbolic link for storage
php artisan storage:link
