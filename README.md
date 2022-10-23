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

 ```

