---
title: lnstall kernel
description: "lnstall kernel."

---

<div class="Alert Alert--nuxt-green">

<b>ubuntu lnstall kernel Devel</b>

</div> 

https://www.cnblogs.com/acm-jing/p/8604200.html

- **kernel-devel is a RedHat and derivatives package. In Ubuntu you may need to install the linux-kernel-headers and kernel-package. Try the following command in Terminal:**

        sudo apt-get install linux-kernel-headers kernel-package



<div class="Alert Alert--nuxt-green">

<b>ubuntu lnstall Kernel Headers</b>

</div>

https://www.tecmint.com/install-kernel-headers-in-ubuntu-and-debian

- **Install Kernel Headers in Ubuntu and Debian**

- **First check your installed kernel version as well as kernel header package that matches your kernel version using following commands.**

        uname -r
        apt search linux-headers-$(uname -r)

- **On Debian, Ubuntu and their derivatives, all kernel header files can be found under /usr/src directory. You can check if the matching kernel headers for your kernel version are already installed on your system using the following command.**

        $ ls -l /usr/src/linux-headers-$(uname -r)

- **From the above output, it’s clear that the matching kernel header directory doesn’t exist, meaning the package is not yet installed.**

- **Before you can install the appropriate kernel headers, update your packages index, in order to grab information about the latest package releases, using the following command.**

        sudo apt update

- **Then run the following command that follows to install the Linux Kernel headers package for your kernel version.**

        sudo apt install linux-headers-$(uname -r)

- **That’s all! In this article, we have explained how to install kernel headers in Ubuntu and Debian Linux and other distributions in the Debian family tree.**

- **Always keep in mind that to compile a kernel module, you will need the Linux kernel headers. If you have any quires, or thoughts to share, use the comment form below to reach us.**