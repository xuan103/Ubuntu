# 系統更新指令

> 前提是 Linux 要連上網路，以及取得root權限，以下sudo指令就是用來取得root權限的!

<div class="Alert Alert--nuxt-green">

<b>步驟：</b>

</div>

- **指令一：用來取得遠端更新伺服器的套件檔案清單。**
<br>sudo apt-get update。

- **指令二：更新套件。**
<br>sudo apt-get -y dist-upgrade

- **指令三：清除更新時所下載回來的更新(安裝)檔案。**
<br>sudo apt-get clean

