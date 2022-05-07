# Create-Template
A command line util to add minimal boilerplate code for oranisation to new files

## Ussage:
### Syntax:

Create file
```
create <yourfile>.py
         |-----> .c
         |-----> .cpp
         |-----> .go
         |-----> .html
         |-----> .java
         |-----> .js
         |-----> .kotlin
         |-----> .rs
         |-----> .sh
         |-----> .zsh
         '-----> .fish

```
</br>
Populate existing empty file
```
create -p <yourfile>.py
             |-----> .c
             |----->  .cpp
             |----->  .go
             |----->  .html
             |----->  .java
             |----->  .js
             |----->  .kotlin
             |----->  .rs
             |----->  .sh
             |----->  .zsh
             '----->  .fish
```

### Examples:
```bash
$ create myfile.c
```
```bash
$ create -p myfile.c
```

## Additional
replace touch with create run:
```bash
shell=$(echo $SHELL | awk -F '/' '{print $3}')
echo "###### create ########"
echo "alias touch='create $1'" >> ${shell}rc
```