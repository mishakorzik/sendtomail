## Usage

#### Send free message to email, without your email! It is strictly forbidden to send spam or threats or 18+

```python
# Enable debug for more information
>>> from sendtomail import *
>>> server.debug("on")

# Disable debug for more information
>>> from sendtomail import *
>>> server.debug("off")


# Send free message to email (plain)
>>> from sendtomail import server
>>> server.send("gmail.com", "he1zen@null.net", "plain", "Test subject", "hello, its a test message!")
'200'
>>>

# Send free message to email (html)
>>> from sendtomail import server
>>> server.send("gmail.com", "he1zen@null.net", "html", "Test subject", 
"""<!DOCTYPE html>
<html>
<body>
      <h1> hello, its a test message! </h1>
</body>
</html>""")
'200'
>>>

```

#### Text message <img width="99.9%" src="https://raw.githubusercontent.com/mishakorzik/mishakorzik.menu.io/master/%D0%A1%D0%B5%D1%80%D0%B2%D0%B5%D1%80/Screenshot_2023-01-22-14-44-57-023-edit_com.google.android.gm.jpg"/>

#### Html message <img width="99.9%" src="https://raw.githubusercontent.com/mishakorzik/mishakorzik.menu.io/master/%D0%A1%D0%B5%D1%80%D0%B2%D0%B5%D1%80/Screenshot_2023-01-22-14-48-09-961-edit_com.google.android.gm.jpg"/>

---

```python
# Servers list
>>> from sendtomail import server
>>> regions = server.regions()
>>> print(regions)
SMTP servers: gmail.com, yandex.com, mail.ru
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
download file <a href='https://drive.google.com/file/d/1PjANjknXugxG8wa8TKLsSjhksWXSFFSL/view?usp=share_link'>sendtomail.exe - v4</a>

and start file, i recommend select gmail.com server.

## Tool information

```
## Status codes
200 - Succesfully send
400 - Failed to send
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
gmail.com   - fast - recommend 
yandex.com  - slow - not recommend
mail.ru     - slow - not recommend
```

**there are logs on the server for security purposes**
