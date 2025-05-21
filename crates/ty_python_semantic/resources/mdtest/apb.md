# mytest

## foo

```py
from typing import NoReturn
import sys

def f() -> NoReturn:
    sys.exit(1)

# def g(x: int | None):
#   if x is None:
#     sys.exit(1)
#
#   x + 3
#
# def f():
#   x = 3
#
#   sys.exit(1)
#
#   x = 4
#   reveal_type(x)
#
```

## bar

```toml
[environment]
python-version = "3.12"
```

```py
from ty_extensions import Intersection, is_subtype_of

class A: ...
class B: ...

type ABC = Intersection[A, B]

is_subtype_of(ABC, A)
is_subtype_of(ABC, B)
```
