## Lab 02

- Name: liam o'leary
- Email oleary.23@wright.edu

## Part 1 Answers

Command to SSH to AWS instance:
```
[ssh -i C:\users\olear\labsuser ec2-olear@52.70.100.248]
```

## Part 2 Answers

1. `chmod u+r bubbles.txt`
    - Means: Allows file owner(u) read(r) permissions on the bubbles file
2. `chmod u=rw,g-w,o-x banana.cabana`
    - Means: allows file owner(u) read(r) and write(w) permissions while removing write permissions from the group(g) and removes execute(x) permissions to others(o) 
3. `chmod a=w snow.md`
    - Means: allows all(a) users only writing(w) permissions
4. `chmod 751 program`
    - Means: owner has read(r), write(w), and execute(x) permissions(7), group has read, and write(5), others have execute permissions(1)
5. `chmod -R ug+w share`
    - Means: -R gives user(u) and group(g) write permissions on share

## Part 3 Answers

1. Command to create new user: sudo useradd new_user
2. Path to user's home directory: echo Home
3. Evaluate if `ubuntu` can add files to user's home directory:ls -ld /home/user
4. Command to switch to user:
5. Command(s) to go to user's home directory: cd /home/user
6. Evaluate if user can add files to user's home directory: ls -l /home/user/testfile
7. Command to switch to `ubuntu`: sudo su -ubuntu
8. Command to return to `ubuntu` home directory: cd~

## Part 4 Answers

For each, write the command used or answer the question posed.

1. Command to create group named `crew`: sudo groupadd crew
2. Command(s) to add `ubuntu` & user to group `crew`: sudo usermod -aG crew ubutu, sudo usermod -aG crew new_user
3. Command to modify `share` to have group ownership of `crew`: sudo chown :crew /path
4. Command to switch to user: sudo su -new_user
5. Command to add file to `share`: touch /path.../newfile
6. Evaluate why these steps allowed the above action: the group crew was created, ubuntu user was added to crew, shared directory, crew and others can now add files and share

## Part 5 Answers

For each, write the command used or answer the question posed.

1. Command to create file using `sudo`: sudo touch /path.../file.txt
2. Evaluate (in plain text) the permission of the file: ls -l /path.../file.txt
3. Provide a method to edit the file without modifying permissions: sudo name /path...file.txt
4. Command(s) to modify permissions: sudo chmod u+x /path...file.txt

## Citations

To add citations, provide the site and a summary of what it assisted you with.  If generative AI was used, include which generative AI system was used and what prompt(s) you fed it.
