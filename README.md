# 🚀 Ultimate Laravel Commands Key Guide (The Definitive Cheat Sheet)

A comprehensive, easy-to-understand reference guide for Laravel, PHP, and Composer commands, tailored for quick workflows.

---

## 🧱 1. PHP & Composer (Base Setup)

### 🔑 `php -v`
👉 PHP version check করে।
* **Use:** সিস্টেমে PHP সঠিকভাবে ইনস্টলড এবং কনফিগারড আছে কিনা তা নিশ্চিত করতে।

### 🔑 `composer -V`
👉 Composer version check করে।
* **Use:** Laravel-এর ডিপেন্ডেন্সি ম্যানেজার ঠিকঠাক কাজ করছে কিনা তা দেখতে।

### 🔑 `composer install`
👉 `composer.lock` ফাইল অনুযায়ী প্রজেক্টের সব packages ইনস্টল করে।
* **Use:** নতুন প্রজেক্ট ক্লোন (Clone) করার পর প্রথম কাজ।

### 🔑 `composer update`
👉 `composer.json` অনুযায়ী সব প্যাকেজ লেটেস্ট ভার্সনে আপডেট করে এবং lock ফাইল রিফ্রেশ করে।
* **Use:** প্রজেক্টের ডিপেন্ডেন্সি আপডেট করার জন্য।

---

## 🚀 2. Laravel Project Setup

### 🔑 `composer create-project laravel/laravel project-name`
👉 একদম ফ্রেশ একটি Laravel প্রজেক্ট ডিরেক্টরি তৈরি করে।
* **Use:** নতুন প্রজেক্ট স্ক্র্যাচ থেকে শুরু করার জন্য।

### 🔑 `php artisan serve`
👉 লোকাল ডেভেলপমেন্ট সার্ভার রান করে।
* **Use:** ব্রাউজারে প্রজেক্টটি চালানোর জন্য (Default: `http://127.0.0.1:8000`)।

---

## 🔑 3. App Key & Configuration

### 🔑 `php artisan key:generate`
👉 অ্যাপ্লিকেশনের জন্য একটি সিকিউর ক্রিপ্টোগ্রাফিক কি (AES-256) জেনারেট করে `.env` ফাইলে সেট করে।
* **Use:** প্রজেক্ট ফার্স্ট টাইম সেটআপ এবং ইউজার সেশন ও এনক্রিপশনের নিরাপত্তা নিশ্চিত করতে।

### 🔑 `php artisan config:clear`
👉 কনফিগারেশন ক্যাশ ফাইলটি ডিলিট করে。
* **Use:** `.env` বা `config/` ফোল্ডারের ফাইলে কোনো পরিবর্তন করার পর তা ইনস্ট্যান্টলি অ্যানাবল করতে।

### 🔑 `php artisan config:cache`
👉 সব কনফিগারেশন ফাইলকে একটি একক ফাইলে কম্বাইন করে ক্যাশ করে, যা পারফরম্যান্স বুস্ট দেয়।
* **Use:** **Production Server**-এ মাস্ট ইউজ করতে হবে।

---

## 🗄 4. Database & Migration System

### 🔑 `php artisan migrate`
👉 নতুন এবং পেন্ডিং থাকা সব মাইগ্রেশন ফাইল রান করে ডাটাবেজে টেবিল তৈরি করে।
* **Use:** ডাটাবেজ স্ট্রাকচার আপডেট বা অ্যাপ্লাই করতে。

### 🔑 `php artisan migrate:rollback`
👉 একদম শেষ ধাপে রান হওয়া মাইগ্রেশনগুলোকে আনডু (Undo) করে।
* **Use:** রিসেন্ট কোনো টেবিলে ভুল হলে তা ফিক্স করতে। (নির্দিষ্ট স্টেপ আনডু করতে: `--step=5`)

### 🔑 `php artisan migrate:fresh`
👉 ডাটাবেজের সব টেবিল সম্পূর্ণ ড্রপ (Delete) করে একদম শুরু থেকে আবার সব মাইগ্রেশন রান করে।
* **Use:** ডেভেলপমেন্টের সময় ডাটাবেজ ক্লিন রিসেট করতে।

### 🔑 `php artisan migrate:refresh`
👉 সব মাইগ্রেশন রোলব্যাক করে এবং আবার রান করে।
* **Use:** ডাটাবেজ ড্রপ না করে স্ট্রাকচার রিলোড করতে।

### 🔑 `php artisan migrate:status`
👉 কোন কোন মাইগ্রেশন রান হয়েছে আর কোনগুলো বাকি আছে তার একটি স্ট্যাটাস টেবিল দেখায়।
* **Use:** ডাটাবেজ সিঙ্ক চেক করতে।

---

## 🧱 5. MVC & Core Component Generation (The 'make' Commands)

### 🔑 `php artisan make:model Product`
👉 শুধুমাত্র একটি Eloquent Model তৈরি করে।
* **Use:** ডাটাবেজ টেবিলকে অবজেক্ট-ওরিয়েন্টিড উপায়ে রিপ্রেজেন্ট করতে।

### 🔑 `php artisan make:model Product -m`
👉 Model এবং এর সাথে ডিক্লেয়ারড ডাটাবেজ **Migration** ফাইল একসাথে তৈরি করে।
* **Use:** টেবিল ও মডেলের বেসিক স্ট্রাকচার এক ক্লিকে রেডি করতে।

### 🔑 `php artisan make:model Product -mc`
👉 Model + Migration + **Controller** একসাথে তৈরি করে।
* **Use:** ব্যাকএন্ডের ফুল ফিচার আর্কিটেকচার সেটআপের জন্য।

### 🔑 `php artisan make:model Product -mrcs`
👉 Model + Migration + Resource Controller + Factory + Seeder একসাথে তৈরি করে।
* **Use:** এক কমান্ডে একটি ফিচারের সবকিছু (All-in-one) রেডি করার জন্য।

---

### 🔑 `php artisan make:controller ProductController`
👉 একটি ব্ল্যাংক কন্ট্রোলার ফাইল তৈরি করে।
* **Use:** অ্যাপ্লিকেশনের বিজনেস লজিক হ্যান্ডেল করতে।

### 🔑 `php artisan make:controller ProductController -r`
👉 একটি **Resource Controller** তৈরি করে (CRUD-এর জন্য ইণ্ডেক্স, ক্রিয়েট, স্টোর, শো, এডিট, আপডেট, ডেস্ট্রয় মেথড রেডি থাকে)।
* **Use:** স্ট্যান্ডার্ড CRUD সিস্টেম দ্রুত তৈরি করতে।

### 🔑 `php artisan make:controller ProductController --api`
👉 ক্রিয়েট এবং এডিট মেথড ছাড়া (যা API-তে লাগে না) শুধু API ফ্রেন্ডলি মেথডসহ কন্ট্রোলার তৈরি করে।
* **Use:** RESTful API ডেভেলপমেন্টের সময়।

---

### 🔑 `php artisan make:middleware CheckAdmin`
👉 নতুন একটি মিডলওয়্যার ফিল্টার তৈরি করে।
* **Use:** রিকোয়েস্ট অথেন্টিকেশন বা রোল-বেসড অ্যাক্সেস কন্ট্রোল করতে।

### 🔑 `php artisan make:request StoreProductRequest`
👉 একটি কাস্টম Form Request ক্লাস তৈরি করে।
* **Use:** কন্ট্রোলার থেকে ভ্যালিডেশন লজিক আলাদা করে কোড ক্লিন রাখতে।

---

## 📄 6. Views (Blade Engine)

👉 ভিউ ফাইল ম্যানুয়ালি বা এক্সটেনশনের মাধ্যমে তৈরি করতে হয়:
```text
resources/views/home.blade.php
