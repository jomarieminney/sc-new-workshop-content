---
title: "Installing Laravel Herd"
date: 2025-09-28
weight: 2
---

#### Installing Herd
Choose your operating system below and follow the instructions to get your local server up and running.

{{< tabs groupid="a" >}}
{{% tab title="_**MacOS**_" %}}
 - Go to the [Laravel Herd Website](https://herd.laravel.com).
 - Click the red **Download for MacOS** button
 - _What other steps are required to get to 'open Herd'?_
{{% /tab %}}
{{% tab title="_**Windows**_" %}}
  - Go to the [Laravel Herd Website](https://herd.laravel.com/windows).
  - Click the red **Download for Windows** button
  - Once downloaded, double click the installer to run it. Click **Finish** when complete.

{{% /tab %}}
{{% tab title="_**Linux**_" %}}

If you are using Linux, chances are that you are more comfortable installing and running your own development environment in general. Laravel Herd is not available on Linux but below we've listed the three most common solutions for setting up a local development server for Laravel on Linux.

__Option 1__
 - To install PHP, Composer, and the Laravel installer directly (not using a package manager) run `/bin/bash -c "$(curl -fsSL https://php.new/install/linux/8.4)"`

__Option 2__
 - If you prefer to use your package manager (e.g. apt, dnf, pacman...) you will first need to install `php` and `composer` if you don't already have them. For example, if `apt` is your package manager, run `sudo apt install php` and `sudo apt install composer`. 
 - Once you have PHP and Composer installed, run `composer global require laravel/installer`. Normally using `composer require` will install a composer package to the local project directory, but with the `global` argument it will make the composer package available everywhere, which is needed as this will be used to create the laravel project directory itself! (for example with `laravel new my-app`)

__Option 3__
- If you already use and are familiar with Docker, check out [Laravel Sail](https://laravel.com/docs/12.x/sail).
{{% /tab %}}
{{< /tabs >}}

Next: [Create Your Site](/laravel/creating_first_site/)

