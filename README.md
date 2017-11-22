# (Unofficial) Library MainAPI SMSNotification for Codeigniter 3 

- Special Thank's to Dev Summit Developer 2017 ITB Sabuga Bandung 23-Nov-2017
- Thank's to MainAPI for Amazing this API
# How to Use ?

Usage

``` php
$sms = new Sendsms();
$sms->setClient_id("xxx");
$sms->setSecret_id("xxx");
$sms->setMsdn("081214267695");
$sms->setContent("081214267695");
$res = $sms->sendSMS();
if($res->body->code == 1)
{
   echo "Success";
}else{
    echo "Fail";
}
```
OR Loads as Library
``` php
$this->load->library("sendsms");
$this->sendsms->setClient_id("xxxx");
$this->sendsms->setSecret_id("xxx");
$this->sendsms->setMsdn("xxx");
$this->sendsms->setContent("xxx");
$res = $this->sendsms->sendSMS();
if($res->body->code == 1)
{
   echo "Success";
}else{
    echo "Fail";
}
```


