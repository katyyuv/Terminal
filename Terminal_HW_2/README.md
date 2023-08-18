## Homework 2

### 1. Create a folder dir_1
`mkdir dir_1`

### 2. Go to the folder
`cd dir_1`

### 3. Create a folder inner_dir_1
`mkdir inner_dir_1`

### 4. View user's location
`pwd`

### 5. Create an empty text file tf_1.txt, while in the dir_1 folder
`touch tf_1.txt`

### 6. While in the dir_1 folder, use the cat command to create a text file tf_2.txt with the following lines:
- the first 1
- the second 2
- the third 3
```
cat > tf_2.txt
the first 1
the second 2
the third 3
```

### 7. Go to the inner_dir_1 folder
`cd inner_dir_1`

### 8. Use cat to make a text file tf_3.txt with any lines. 
```
cat > tf_3.txt
Hello!
How are you?
What are you doing?
```

### 9. Use cat to add the line "the second 2" to the text file tf_3.txt
```
cat >> tf_3.txt
the second 2
```

### 10. Use cat to add the line "the sec 2" to the text file tf_3.txt
```
cat >> tf_3.txt
the sec 2
```

### 11. Use cat to add the line "the sec 3" to the text file tf_2.txt
```
cat >> ../tf_2.txt
the sec 3
```

### 12. Use cat to add the line "the SeCoNd 2" to the text file tf_3.txt
```
cat >> tf_3.txt
the SeCoNd 2
```

### 13. Use cat to add the line "the seConD 2" to the text file tf_2.txt
```
cat >> ../tf_2.txt
the seConD 2
```

### 14. Create a text file tf_4.txt with 15 lines in it.
```
 cat > tf_4.txt
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
```

### 15. Create a text file tF_5.txt with 13 lines in it
```
cat > tF_5.txt
1
2
3
4
5
6
7
8
9
10
11
12
13
```

### 16. Display a list of all files in the folder
`ls -la`

### 17. Exit the folder inner_dir_1
`cd ..`

### 18. Display the contents of the file tf_3.txt in the terminal
`cat inner_dir_1/tf_3.txt`

### 19. Find the path to the file tf_4.txt
`find . -name tf_4.txt`

### 20. Clear the file tf_4.txt of its contents without deleting the file itself
`cat > inner_dir_1/tf_4.txt` and press `Ctrl + C`

### 21. Find the path to files that have "tf" in the name
`find . -name "*tf*"`

### 22. Find the path to files that have "tf" in the name and letters in any case.
`find . -iname "*tf*"`

### 23. Find lines in files with the letter combination "sec" in the current folder
`grep sec *`

### 24. Find lines in files where there is a combination of letters "sec" in any case in the current folder
`grep -i sec *`

### 25. Find lines in files with only the letter combination "sec" in the current folder
`grep -w sec *`

### 26. Find lines in files with only the combination of letters "sec" in any case in the current folder
`grep -wi sec *`

### 27. Find lines in files with the letter combination "second" in the current folder
`grep second *`

### 28. Find lines in files where there is a combination of letters "second" in any case in the current folder
`grep -i second *`

### 29. Find lines in files with the letter combination "second" in all folders below the folder level
`grep -r second`

### 30. Find only the path and file name with "second" in the lines in the current folder
`grep -sl second *`

### 31. Find all lines in all files where there is no "second" combination
`grep -rv second`

### 32. Find only the name and path to files where there is no "second" combination
`grep -rL second`

### 33. Display the last 4 lines of any text file in the terminal
`tail -n 4 tf_2.txt`

### 34. Display the first 4 lines of any text file in the terminal
`head -n 4 tf_2.txt`

### 35. One line command. Create a folder and create a text file with the contents
```
mkdir inner_dir_2 && cat > tf_6.txt
1
2
3
4
5
6
```

### 36. One line command. Move text files with the word "sec" in their contents to any single folder
`grep -rl 'sec' | xargs-I{} mv {} inner_dir_2`

### 37. One line command. Copy text files with the word "sec" in their contents to any one folder
`grep -rl 'sec' | xargs -I{} cp {} inner_dir_1`

### 38. One line command. Find all lines with "sec" in all text files, copy and paste these lines into one new created text file
`grep -rh "sec" | xargs -I{} echo {} > tf_6.txt`

### 39. One line command. Delete text files with the word "sec" in their contents
`grep -rl "sec" | xargs -I{} rm {}`

### 40. Just display the line "Good job!!!" in the terminal
`echo Good job!!`
