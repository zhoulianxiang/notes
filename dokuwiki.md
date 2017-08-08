https://www.dokuwiki.org/

## get

一般我喜欢 Stable (Recommended)

    wget https://download.dokuwiki.org/src/dokuwiki/dokuwiki-stable.tgz

### apache2 & php5

    sudo apt-get install apache2 php5

## install

https://www.dokuwiki.org/install

    tar -xvvf dokuwiki-stable.tgz
    sudo cp -r dokuwiki-2017-02-19b/ /var/www/html/zwiki
    sudo chown -R www-data:www-data /var/www/html/zwiki

从浏览器访问 `http://<wiki_host>/zwiki/install.php`

设置wiki，用默认设置即可

## login

用刚刚设置的管理员账号登录，开始设置

### Admin -> User Manager

增加一个非admin日常用户

### Admin -> Configuration Settings

常用的设置

- Display->youarehere
    - enable
- Display->fullpath
    - enable
- Advanced->fnencode
    - utf-8
- Advanced->userewrite
    - .htaccess
- Advanced->useslash
    - enable

#### Advanced->userewrite

- https://www.dokuwiki.org/rewrite

##### 设置apache2 rewrite

    sig3@zpi:/etc/apache2 $ vim apache2.conf

```
164 <Directory /var/www/>
165     Options Indexes FollowSymLinks
-166     AllowOverride None
+166     AllowOverride All
167     Require all granted
168 </Directory>
```

    sig3@zpi:/etc/apache2 $ sudo a2enmod rewrite
    sig3@zpi:/etc/apache2 $ sudo service apache2 restart

## secure

https://www.dokuwiki.org/security

个人使用，我不是很在意这个告警

## tips

-  设置发布邮件提醒，会导致保存延迟。
