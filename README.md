# log ip
logging ip, OS, browser, time and file .php in a file. Database less. 

### log format exsample
```
From NL, South Holland, Krimpen aan den IJssel, AS43350 NForce Entertainment B.V. Client: Windows 10---Firefox(78.0), ip: 46.166.139.*, at 2021-08-20 18:35:40 access to: /logipgithub/index.php
From US, Delaware, Wilmington, AS208294 CIA TRIAD SECURITY LLC Client: Windows 10---Firefox(78.0), ip: 2a0b::*, at 2021-08-20 18:36:30 access to: /logipgithub/index.php
From US, Arizona, Mesa, AS62744 Quintex Alliance Consulting Client: Windows 10---Firefox(78.0), ip: 2620:7:6001::*, at 2021-08-20 18:37:06 access to: /logipgithub/index.php
From US, Arizona, Mesa, AS62744 Quintex Alliance Consulting Client: Windows 10---Firefox(78.0), ip: 2620:7:6001::*, at 2021-08-20 18:37:45 access to: /logipgithub/comm_function.php
From AT, Styria, Graz, AS208323 Foundation for Applied Privacy Client: Windows 10---Firefox(78.0), ip: 2a03:e600::*, at 2021-08-20 18:37:58 access to: /logipgithub/comm_function.php
```
### if use cloudflare CDN make sure below code is uncommented
```
if (isset($_SERVER["HTTP_CF_CONNECTING_IP"])) {
  $_SERVER['REMOTE_ADDR'] = $_SERVER["HTTP_CF_CONNECTING_IP"];
}
```
