https://www.dokuwiki.org/

## get

一般我喜欢 Stable (Recommended)

    wget https://download.dokuwiki.org/src/dokuwiki/dokuwiki-stable.tgz

### apache2

    sudo apt-get install apache2

### php5

    sudo apt-get install php5

## install

https://www.dokuwiki.org/install

    tar -xvvf dokuwiki-stable.tgz
    sudo cp -r dokuwiki-2017-02-19b/ /var/www/html/zwiki
    sudo chown -R www-data:www-data /var/www/html/zwiki

从浏览器访问 `http://<wiki_host>/zwiki/install.php`

设置wiki，用默认设置即可

## login

用刚刚设置的管理员账号登录，开始设置

### user

私人wiki，就一个管理员账户就可以了

### Admin -> Configuration Settings

常用的设置

#### Advanced->Use nice URLs

- https://www.dokuwiki.org/rewrite
- ...
