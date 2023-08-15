# Use Linux commands to manage file permissions

Scenario

You are a security professional at a large organization. You mainly work with their research team. Part of your job is to ensure users on this team are authorized with the appropriate permissions. This helps keep the system secure. 

Your task is to examine existing permissions on the file system. You’ll need to determine if the permissions match the authorization that should be given. If they do not match, you’ll need to modify the permissions to authorize the appropriate users and remove any unauthorized access.

Current file permissions

This displays the file structure of the /home/researcher2/projects directory
and the permissions of the files and subdirectory it contains.

In the /home/researcher2/projects directory, there are five files with the following
names and permissions:

● project_k.txt
  ○ User = read, write,
  ○ Group = read, write
  ○ Other = read, write
● project_m.txt
  ○ User = read, write
  ○ Group = read
  ○ Other = none
● project_r.txt
  ○ User= read, write
  ○ Group = read, write
  ○ Other = read
● project_t.txt
  ○ User = read, write
  ○ Group = read, write
  ○ Other = read
● .project_x.txt
  ○ User = read, write
  ○ Group = write
  ○ Other = none

There is also one subdirectory inside the projects directory named drafts. The
permissions on drafts are:

● User = read, write, execute
● Group = execute
● Other = none
