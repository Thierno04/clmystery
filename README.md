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
cd ..
```
```bash 
cd interviews/
grep "AAA" *
cat interview-290346
cd ..
```
```bash
ls
grep "Annabel" people
grep "Annabel.*F" people
grep "Annabel.*F\s" people
grep "Church" people
```
```bash
awk '{print NR "- " $0}' people
awk 'END {print NR}' people
cut -d, -f 2 people
cut -d, -f 1- people --output-delimiter=" | "
cut -d, -f 1- people --output-delimiter=" : "
awk 'NF==0 {print NR}' people
```
```bash
man grep
grep "\w\s\w\n" new_memberships
grep ".*\s.*\n" new_memberships
grep "\w*\s\w*\n" new_memberships
``` 
```bash
cd interviews/
grep "Sun" *
grep "Church" *
cd ..
head -n 173 streets/Mattapan_Street | tail -n 1
ls interviews/
cat interviews/*9437737
grep "L337" vehicles
grep -A 5 "L337" vehicles
```
```bash
cd memberships/
cat Fitness_Galaxy AAA United_MileagePlus | grep "John Smith"
cat Fitness_Galaxy AAA United_MileagePlus | grep -c "John Smith"
cat Fitness_Galaxy AAA United_MileagePlus | grep "John Smith" | wc -l
cat Fitness_Galaxy AAA United_MileagePlus | grep "Erika Owens" | wc -l
cat Fitness_Galaxy AAA United_MileagePlus | grep "Aron Pilhofer" | wc -l
cat Fitness_Galaxy AAA United_MileagePlus | grep "Miranda Mulligan" | wc -l
cat Fitness_Galaxy AAA United_MileagePlus | grep "Joe Germuska" | wc -l
cat Fitness_Galaxy AAA United_MileagePlus | grep "Jeremy Bowers" | wc -l
cat Fitness_Galaxy AAA United_MileagePlus | grep "Jacqui Maher" | wc -l
cat Delta_SkyMiles AAA Museum_of_Bash_History | grep "Jacqui Maher" | wc -l
cat Delta_SkyMiles AAA Museum_of_Bash_History | grep "Jeremy Bowers" | wc -l
cat Delta_SkyMiles AAA Museum_of_Bash_History | grep "Joe Germuska" | wc -l
cat Delta_SkyMiles AAA Museum_of_Bash_History | grep "Miranda Mulligan" | wc -l
cat Delta_SkyMiles AAA Museum_of_Bash_History | grep "Aron Pilhofer" | wc -l
cat Delta_SkyMiles AAA Museum_of_Bash_History | grep "Erika Owens" | wc -l
cat Delta_SkyMiles AAA Museum_of_Bash_History Terminal_City_Library| grep "Erika Owens" | wc -l
cat Delta_SkyMiles AAA Museum_of_Bash_History Terminal_City_Library| grep "Aron Pilhofer" | wc -l
cat Delta_SkyMiles AAA Museum_of_Bash_History Terminal_City_Library| grep "Miranda Mulligan" | wc -l
cat Delta_SkyMiles AAA Museum_of_Bash_History Terminal_City_Library| grep "Joe Germuska" | wc -l
cat Delta_SkyMiles AAA Museum_of_Bash_History Terminal_City_Library| grep "Jeremy Bowers" | wc -l
cat Delta_SkyMiles AAA Museum_of_Bash_History Terminal_City_Library| grep "Jacqui Maher" | wc -l
cd ..
```
```bash
ls
cd interviews/
grep "Maher" *
echo "The culprit is Jeremy Bowers"
```
 
