### tablib
---
https://github.com/kennethreitz/tablib

```py
headers = ('first_name', 'last_name')

data = [
  ('John', 'Adams'),
  ('Goorge', 'Washington')
]

data = tablib.Dataset(*data, headers=headers)

data.append(('Henry', 'Ford'))

data.append_col((90, 67, 83), header='age')

print(data[:2])
print(data['first_name'])
del data[1]

print(data.export('json'))
print(data.export('yaml'))
print(data.export('csv'))
with open('people.xls', 'wb') as f:
print(data.export('df')):
```

```sh
pip install tablib[pandas]
```

```
```

