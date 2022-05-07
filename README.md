# Create-Template
A command line util to add minimal boilerplate code for oranisation to new files

## Installation:
```bash
git clone https://github.com/NewDawn0/create-templates.git
cd create-templates
mv create /usr/local/bin/
mkdir -p $HOME/.ndos/create/
mv templates/* $HOME/ndos/create/
```
</br>

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


### Examples:
```bash
create myfile.c
```
Or if executed the optional command down below
```bash
touch myfile.c
```
</br>

## Optional
replace touch with create run:
```bash
shell=$(echo $SHELL | awk -F '/' '{print $3}')
echo "###### create ########"
echo "alias touch='create $1'" >> ${shell}rc
```
