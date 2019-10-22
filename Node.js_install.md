# 版本需求 ex:
- **nodejs 4.2.6**
- **npm  6.9.0**
- **node 10.16.3**

<a href>"https://blog.gtwang.org/web-development/install-node-js-in-windows-mac-os-x-linux/?fbclid=IwAR38BJ6v_k3iNk37CEhuwJYmO6EmSkNqBnA3KYLPNqlpMBALeroAHv7fh04"</a>

# 下載 Node.js 二進位檔安裝

- **如果是在 Linux 系統下要安裝 Noode.js，可以從 Node.js 的官方網站下載編譯好的二進位版本（Linux Binaries），解壓縮之後就可以使用了。例如：**

        wget http://nodejs.org/dist/v10.16.3/node-v10.16.3-linux-x64.tar.gz

        tar zxf node-v10.16.3-linux-x64.tar.gz


- **接著把解壓縮出來的 node-v0.10.23-linux-x64 目錄放到想要安裝的位置就行了，常見的方式是把它放在 /opt 下面，就像這樣：**

        sudo mv node-v10.16.3-linux-x64 /opt/

- **而 node 與 npm 這兩個指令就存放在其中的 bin/ 這個目錄中，加上絕對路徑即可執行，例如：**

        /opt/node-v10.16.3-linux-x64/bin/node -h

- **如果要讓使用上更方便，也可以把這個路徑加入 PATH 中：**

        export PATH=$PATH:/opt/node-v10.16.3-linux-x64

- **如果要讓每次登入都會自動設定 PATH，可以把上面這行加在自己的 ~/.bashrc 中：**

        echo 'PATH=$PATH:/opt/node-v10.16.3-linux-x64' >> ~/.bashrc

# 使用 apt 安裝 Node.js

- **在 Ubuntu Linux 中，也可以透過 apt 來安裝：**

        sudo apt-get install nodejs

# 從 Node.js 原始碼編譯安裝

- **如果想要拿 Node.js 的原始碼自己編譯安裝的話，因為它在編譯的時候會需要 Python 2.6 或 2.7 版，所以請檢查自己的 Python 版本是否符合需求：**

        python --version

- **輸出會像這樣**
        
        Python 2.7.

- **如果你的 Python 版本太舊，就要先把 Python 更新才行。接著下載 Node.js 的原始碼：**

        wget http://nodejs.org/dist/v10.16.3/node-v10.16.3.tar.gz

- **解壓縮之後，進入目錄中執行 configure：**

        tar xvf node-v10.16.3.tar.gz
        cd node-v10.16.3/
        ./configure

- **configure 提供的選項很多，可以使用 --help 參數查看：**

        ./configure --help

- **最常用的應該是指定安裝路徑，如果要把安裝路徑指定為 /opt/nodejs，則使用**

        ./configure --prefix=/opt/nodejs

- **接著執行 make 進行編譯：**

        make

- **如果編譯沒問題，就可以安裝了：**

        sudo make install

- **安裝完成後，再測試一下：**

        /opt/nodejs/bin/node -h

- **如果不想每次都要加上絕對路徑，就仿照上面的做法，把它加入 PATH 就可以了。**

        export PATH=$PATH:/opt/nodejs/bin

- **或是直接放進 ~/.bashrc：**

        echo 'PATH=$PATH:/opt/nodejs/bin' >> ~/.bashrc





