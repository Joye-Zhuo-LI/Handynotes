
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
