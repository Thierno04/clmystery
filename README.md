# The Command Line Murders
```bash
cd mystery/
cat crimescene
wc -l crimescene
head -n 20 crimescene
head -n 100 crimescene
ls
```
##### I send the output to a new file "clue_list"
```bash
cat crimescene | grep -C10 "CLUE"
cat crimescene | grep -C5 "CLUE" > clue_list
cat clue_list
cat crimescene | grep -C3 "6'" > six_least
cat six_least
 ```
##### Different witnesses
```bash
cat crimescene | grep -C3 "AAA"
cat crimescene | grep -C3 "SkyMiles"
cat crimescene | grep -C3 "library"
```
##### Questions
```bash
cat clue_list
cat crimescene | grep -iC3 "Annabel"
cat crimescene | grep -iC3 "spiky"
cat crimescene | grep -iC10 "Zealand"
```
##### I display and sort the memberships file to a new file new_memberships
```bash 
cd memberships/
ls
cat AAA
cat AAA Delta_SkyMiles Museum_of_Bash_History|sort > new_memberships
cat new_memberships
grep "\w* \w*\n" new_memberships
grep "\w* \w*\n" new_memberships
grep "\w* \w*\n" new_memberships
grep "\w* \w*\n\r" new_memberships
grep "\w* \w*\r" new_memberships
grep ".*" new_memberships
grep "\w* \w*${3}" new_memberships
grep "\w* [A-Z][a-z]*\n" new_memberships
```
```bash
awk '{print NF, $0}' new_memberships
uniq -cd new_memberships
uniq -cd new_memberships|grep '^ *3'
uniq -cd new_memberships|grep '^ *3'>new_memberships_2
cat new_memberships_2
uniq -cd new_memberships|grep '^ *4'>new_memberships_4
cat new_memberships_4
cat AAA Delta_SkyMiles Museum_of_Bash_History Terminal_City_Library |sort > new_memberships_4
cat new_memberships_4
rm -r new_memberships_2

```
