## Usage

#### Send free message to email, without your email!

```python
# Send free message to email, debug OFF
>>> from sendtomail import *
>>> server.send("ua", "he1zen@null.net", "hello, its a test message!")
b'200'
>>>

# Send free message to email, debug ON
>>> from sendtomail import *
>>> server.debug("on")
>>> server.send("ua", "he1zen@null.net", "hello, its a test message!")
[3%] Debug mode ON
[7%] Region ua
[11%] Starting to get URL
[20%] Getting json from URL
[40%] URL json data decode
[60%] Server IP 18.189.106.45
[80%] Server connected!
[100%] Data send to server
b'200'
>>>

# Servers list
>>> from sendtomail import *
>>> regions = server.regions()
>>> print(regions)
SMTP regions: tr, ru, ua, us, uk, de, fr, it
>>>

```

```
## Status codes
200 - Succesfully send
400 - bad options
429 - Try in 1 day or choose another region
500 - Internal Server Error
503 - Service Unavailable
504 - Try another region

## Servers Country
tr - turkey
ru - russia
ua - ukraine
us - united states
uk - united kingdom
de - germany
fr - france
it - italia
```

**I also want to inform you that it is possible to send letters from one region to another, for example from Ukraine to USA**
