# The Command Line Murders
```bash
cd mystery/
cat crimescene
wc -l crimescene
head -n 20 crimescene
head -n 100 crimescene
ls
```
I send the output to a new file "clue_list"
```bash
cat crimescene | grep -C10 "CLUE"
cat crimescene | grep -C5 "CLUE" > clue_list
cat clue_list
cat crimescene | grep -C3 "6'" > six_least
cat six_least
 ```
Different witnesses
```bash
cat crimescene | grep -C3 "AAA"
cat crimescene | grep -C3 "SkyMiles"
cat crimescene | grep -C3 "library"
```
Questions
```bash
cat clue_list
cat crimescene | grep -iC3 "Annabel"
cat crimescene | grep -iC3 "spiky"
cat crimescene | grep -iC10 "Zealand"
```
