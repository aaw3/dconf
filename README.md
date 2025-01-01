# Unofficial dconf module

- Supports primary dconf commmands
- Returns list objects as lists
- Uses ast library to convert string to literal types for processing
- Provides watch callback function to obtain new values of changed keys from path

### dconf_utils.py
Contains dconf functions for absolute paths
```python
from dconf_utils import list_subfolders
sub_folders = list_subfolders('/com/github/wwmm/easyeffects/streamoutputs')
```

### dconf_wrapper.py
Contains dconf functions for relative paths
```python
dconf_easyeffects = dconf('com/github/wwmm/easyeffects')
subfolders = dconf_easyeffects.list_subfolders('streamoutputs')
```
