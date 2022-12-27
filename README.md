# yamlutils
A super simple utility library [and cli] to modify yaml files.

## Merge by key
Ever wanted to merge a yaml with an array so that elements of the array would get merged based on some key like `name`?
Use `yamlutils merge-by-key --key 'name' file0.yaml file1.yaml [file2.yaml ...]`.

### Example
file0.yaml:
```
people:
 - name: John
   age: 62
```
file1.yaml:
```
people:
 - name: John
   occupation: Farmer
```
output:
```
people:
 - name: John
   age: 62
   occupation: Farmer
```
