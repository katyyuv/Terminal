## Homework 1

### 1. View user's location
`pwd`

### 2. Create a folder
`mkdir dir`

- Create subfolder `mkdir -p dir_4/dir_5/dir_6`

### 3. Go to the folder
`cd dir`

### 4. Create 3 folders
`mkdir dir_1 dir_2 dir_3`

### 5. Go to any folder
`cd dir_2`

### 6. Create 5 files (3.txt, 2.json)
`touch 1.txt 2.txt 3.txt 1.json 2.json`

- You can also create a file and write something there right away
  ```
  cat > 4.txt
  Hello, world!
  ```
  Press `Ctrl+D` to save and exit


### 7. Create 3 folders
`mkdir dir_2_1 dir_2_2 dir_2_3`

### 8. List the contents of a folder
`ls`

- Displaying the contents of a folder with hidden files `ls -la`

### 9. Open any txt file
`vim 2.txt`

- Open file `cat 2.txt` (view only, no editing)
- You can also open for editing directly in the console: `cat >> 2.txt`

### 10. Write something in this txt file
```
Hello!
How old are you?
Where are you from?
```

### 11. Save and exit
Click on the `[Esc]` button and enter `:wq`

### 12. Exit the folder one level up
`cd ..`

- Change to the previous working directory `cd -`

### 13. Move any 2 created files to any other folder
`mv dir_2/2.txt dir_2/2.json dir_1`

### 14. Copy any 2 created files to any other folder
`cp dir_1/2.txt dir_1/2.json dir_3`

### 15. Find file by name 
`find . -name 2.txt`

### 16. View content in real-time
`grep -i how dir_1/2.txt`

- Case-sensitive word search in a file `grep word 2.txt`
- with `-i` case insensitive word search in a file
- with `-v` displays lines that do not contain queries
- with `-c` displays lines containing the search query
  
### 17. Display the first few lines from a txt file
`head -n 2 dir_1/2.txt`

- Default output of the first 10 lines `head -n dir_1/2.txt`

### 18. Display the last few lines from a txt file
`tail -n 2 dir_1/2.txt`

- Default output of the last 10 lines `tail -f dir_1/2.txt`

### 19. View the contents of a long file
`less dir_1/2.txt`

### 20. Display date and time
`date`

## Task *
### 1. Send http request http://162.55.220.72:5006/terminal-hw-request to server

Request:

`curl http://162.55.220.72:5006/terminal-hw-request`

Response:
```
  "Intro": "Hello!! This is your first response from the server",
  "Tasks": {
    "Task_1": "Send the next URL in terminal: http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number)",
    "result": [
      "Your_String",
      "Your_number"
    ]
  }
}
```

Request:

`curl 'http://162.55.220.72:5006/get_method?name=Kate&age=21'`

Response:
```
[
  "Kate",
  "21"
]
```

### 2. Write a script that will automatically execute steps 3, 4, 5, 6, 7, 8, 13

