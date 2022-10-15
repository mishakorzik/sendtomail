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
>>> from sendtomail import *
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
>>> from sendtomail import *
>>> regions = server.regions()
>>> print(regions)
SMTP servers: gmail.com, outlook.com, yandex.com, mail.ru
>>>

# Get Free SMTP, POP3, IMAP email
>>> from sendtomail import *
>>> server.mail()
{'google-mail': 'qcp9ex.iqu0@gmail.com', 'google-pass': 'dmxsdxqgvlcypitf'}
>>>

# Free email checker
>>> from sendtomail import *
>>> server.validate("he1zen@null.net")
'valid'
>>>

```

## For Windows

download file <a href='https://drive.google.com/file/d/1njyyb_LJHnQznPHg9wn1NJ0s3oIgWwHv/view?usp=sharing'>sendtomail.exe</a>
and start file, im recommend select gmail.com server.

## Tool information

```
## Status codes
200 - Succesfully send
400 - Failed to send, choose another server
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
gmail.com   - 50-70ms - recommend
outlook.com - 60-80ms - not recommend
mail.ru     - 70-90ms - not recommend
yandex.com  - 80-95ms - not recommend
```

**there are logs on the server for security purposes**
