[//]: # (![alt text]&#40;1-9.PNG&#41;)
<!-- https://gist.github.com/rxaviers/7360908 -->
# python snippets for everyone
made with 💜 by [Sina Abedi](https://stackoverflow.com/users/10606346/sina-abedi?tab=profile)


## system programming

### Taking ScreenShot
**Requirement:**
```shell
pip3 install pillow
```

**Code:**
```python
import PIL.ImageGrab as PIG
scr = PIG.grab().save('scr.png')
```

### ‌Print colored text
**Requirement:**
```shell
pip3 install termcolor
```

**Code:**
```python
from termcolor import colored
print(colored('hello', 'red'))
```

### Print real time
**Code:**
```python
import datetime
print(datetime.datetime.now())
```

### Create QRcode
**Requirement:**
```shell
pip3 install qrcode
```

**Code:**
```python
import qrcode

img = qrcode.make('your text')
img.save("qr.png")
```

### Download file
**Requirement:**
```shell
pip3 install wget
```

**Code:**
```python
import wget

wget.download('http://site.com/song.mp3')
```

### Print the value of laptop battery
**Requirement:**
```shell
pip3 install psutil
```

**Code:**
```python
import psutil

print(str(psutil.sensors_battery()[0]), '%')
# output: 74 %‌
```

### Converting image formats
**Requirement:**
```shell
pip3 install pillow 
```

**Code:**
```python
from PIL import Image

img = Image.open("a.png")
img.convert('RGB').save('a.jpg')
```

### Writing in exel file
**Requirement:**
```shell
pip3 install openpyxl
```

**Code:**
```python
from openpyxl import Workbook
wb = Workbook()

# col : 3   row : 5
wb.active['C5'] = 'your string'
wb.save("output.xlsx")
```
