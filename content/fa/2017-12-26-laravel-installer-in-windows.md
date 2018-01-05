---
utid: 20171226124738
date: 2017-12-26 18:47:38
title: آموزش نصب لاراول روی ویندوز در ۵ دقیقه!
_index: laravel-installer-in-windows
categories:
  - webDesign
tags:
  -
---
![Laravel](laravel.png)
در این آموزش در مورد نصب لاراول روی ویندوز میگم. نصب Laravel روی ویندوز مطابق [Document](https://laravel.com/docs/5.5#installing-laravel) خودش از دو روش با استفاده از composer انجام میشه. حتما قبل از شروع این آموزش composer را نصب کنید. (آموزش های فارسی نصب [composer](https://getcomposer.org/) زیاده و می تونید از حضرت Google کمک بگیرید!)

## روش اول استفاده از Laravel installer:

این روش را خودم خیلی دوست دارم و راحت ترین و سریع ترین راه برای نصب لاراول است و شما یک بار لاراول را روی composer نصب می کنید و بعدش هرچندتا application خواستید باهاش می سازید!!

۱ – ابتدا CMD یا Windows powerShell رو باز کنید و این commad را اجرا کنید:

```sh
composer global require "laravel/installer"
```
خب حالا لاراول روی composer نصب شد. برای دسترسی به آن در CMD و PowerShell باشد env ویندوز را ویرایش کنید. از طریق منوی Start عبارت env را جستجو کنید و Edit the system environment variables را باز کنید.
![windows env](env.png)
۲ – در بخش System Variables مقدار Path را انتخاب کنید و گزینه Edit را بزنید و بعد مقدار زیر رو به انتهای مقدار Path اضافه کنید. توجه کنید بجای YOUR_USERNAME_HERE باید username ویندوز خودتون رو بنویسید:
```sh
;C:\Users\YOUR_USERNAME_HERE\AppData\Roaming\Composer\vendor\bin
```
خب حالا هرجایی که میخواین Laravel رو نصب کنید میتونید CMD یا PowerShell را در اون فولدر باز کنید و commad زیر رو اجرا کنید. مثلا من معمولا داخل فولدر C:\Apache24\htdocs لاراول را نصب میکنم.
![CMD](cmd.png)
با اجرای این دستور فولدر جدیدی بنام blog ساخته میشه.

## روش دوم استفاده از Composer Create-Project:

در این روش هربار که شما قصد نصب laravel رو دارید باید با استفاده از CMD یا PowerShell به فولدر مورد نظر برید و دستور زیر را اجرا کنید تا Laravel دانلود و نصب بشه! توصیه میکنم روش اول رو استفاده کنید.

```
composer create-project --prefer-dist laravel/laravel blog
```