
## Roload Package

```python 
import importlib
importlib.reload(you_package)
```

## Add Path
```python 
import sys
module_dir ="modules/"
if module_dir not in sys.path:
    sys.path.insert(0, module_dir)
```

## Relative Path
```python 
from os import getcwd
filePath = f"{getcwd()}/modules/"
```


## Disable SSL Verfication 

### Global 

```python 
import os
import warnings
warnings.filterwarnings("ignore")
os.environ["REQUESTS_CA_BUNDLE"] = ""
os.environ["CURL_CA_BUNDLE"] = ""
```

### Once
```python 
import reqests
requests.get(url,verify = False)
```

## inspect code 
```python 
import module
import inspect
src = inspect.getsource(module)
print(src)
```

## Convert string to datetime
```python 
from datetime import datetime
#Fri Nov 20 19:40:26 +0000 2020
df['date'] = [datetime.strptime(item, '%a %b %d %H:%M:%S +0000 %Y') for item in df['date']  ]
```
## Create requirement.txt for a python project
``` 
pipreqs --encoding=utf8 /GitHub/FolderName/
```
