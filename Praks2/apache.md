# Apache2

## Paigaldamine

Apache2 paigaldamiseks sisestasin käsu
```
apt-get apache2
```
peale seda muudan index.html
```
sudo nano /var/www/html/index.html
```

```
<!DOCTYPE HTML>
<html>
<meta charset="UTF-8">
<body>
<p>Frank Karrp</p>
<p>ISP217</p>
<p>frank.karro@khk.ee
ISP217</p>
</body>
</html>
```
Tavakasutajale avaliku kausta tegemine:
```
mkdir /home/it/public_html.
```
Loon sümboolse linki /var/www kaustaga kasutades käsku:
```
ln -s /home/it/public_html./ /var/www
```
Luban kasutaja kaustad:
```
a2enmod userdir
```
Restart apache2:
```
service apache2 restart
```
