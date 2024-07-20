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
