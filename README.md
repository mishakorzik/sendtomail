## Usage

#### Send free message to email, without your email! It is strictly forbidden to send spam or threats or 18+

## For linux

```python
# Send free message to email, debug OFF
>>> from sendtomail import *
>>> server.send("gmail.com", "he1zen@null.net", "hello, its a test message!")
'200'
>>>

# Send free message to email, debug ON
>>> from sendtomail import server
>>> server.debug("on")
>>> server.send("gmail.com", "he1zen@null.net", "hello, its a test message!")
[3%] Debug mode ON
[7%] Server gmail.com
[11%] Starting to get URL
[20%] Getting json from URL
[40%] URL json data decode
[60%] Server IP he1zen-server.ddns.net:17632
[80%] Server connected!
[98%] Data send to server
'200'
>>>

# Servers list
>>> from sendtomail import server
>>> regions = server.regions()
>>> print(regions)
SMTP servers: gmail.com, outlook.com, yandex.com, mail.ru
>>>

# Get Free SMTP, POP3, IMAP email
>>> from sendtomail import server
>>> server.mail()
{'google-mail': 'qcp9ex.iqu0@gmail.com', 'google-pass': 'dmxsdxqgvlcypitf'}
>>>

# Free email checker
>>> from sendtomail import server
>>> server.validate("he1zen@null.net")
'valid'
>>>

# Send custom data
>>> from sendtomail import server
>>> custom.data("^38^92%72^92%65^92%10")
'\nlocation  : Ukraine\nServer IP : 185.16.36.136\ncreator   : He1Zen, mishakorzik\nmirror    : Europe, amazon\nping      : 50-70ms\n'
>>> 

```

### Server Information

```

# get server info with print
>>> from sendtomail import server
>>> server.info(False)
location: Ukraine
creator: He1Zen, mishakorzik
mirror: Europe, amazon
ping: 50-70ms
>>> 

# get server info with return
>>> from sendtomail import server
>>> server.info(True)
'\nlocation  : Ukraine\nServer IP : 185.16.36.136\ncreator   : He1Zen, mishakorzik\nmirror    : Europe, amazon\nping      : 50-70ms\n'
>>> 

```

### Temp Mail Creation

```python
# Create temp mail
>>> from sendtomail import tempmail
>>> tempmail.create()
'qwm5cn282k55sp@dcctb.com'
>>> 

# Read last message from temp mail
>>> from sendtomail import tempmail
>>> tempmail.read("qwm5cn282k55sp", "dcctb.com")
mailbox is empty
>>> 

```

## For Windows

download file <a href='https://drive.google.com/file/d/1njyyb_LJHnQznPHg9wn1NJ0s3oIgWwHv/view?usp=sharing'>sendtomail.exe - v1</a>
download file <a href='https://drive.google.com/file/d/1Nro-hUV63g0vjS8A135XSWPeEuwePdvx/view?usp=drivesdk'>sendtomail.exe - v2</a>
download file <a href='https://drive.google.com/file/d/1jErK0PHP8yOazigiIh-TGUMRaBdesmIQ/view?usp=drivesdk'>sendtomail.exe - v3</a>

and start file, i recommend select gmail.com server.

## Tool information

```
## Status codes
200 - Succesfully send
400 - Failed to send, choose another server
401 - bad request or wrong command
403 - Email protected or secured
404 - Email not found, try another email
429 - Server error, choose another server
500 - Internal Server Error, try again later
503 - Service Unavailable, try again later
504 - Try another server

## Other codes
valid   - mailbox exists
invalid - mailbox does not exist
timeout - mailbox is unknown


## Services
gmail.com   - 40-60ms - recommend 
yandex.com  - 55-80ms - not recommend
outlook.com - 60-75ms - not recommend
mail.ru     - 70-90ms - not recommend
```

**there are logs on the server for security purposes**
