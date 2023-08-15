# Use Linux commands to manage file permissions

Scenario

You are a security professional at a large organization. You mainly work with their research team. Part of your job is to ensure users on this team are authorized with the appropriate permissions. This helps keep the system secure. 

Your task is to examine existing permissions on the file system. You’ll need to determine if the permissions match the authorization that should be given. If they do not match, you’ll need to modify the permissions to authorize the appropriate users and remove any unauthorized access.

Project description:
In this task, we're going to inspect the current permissions of files and directories in the /home/researcher2/projects directory and adjust them if necessary, ensuring that only authorized users and groups have the necessary permissions, while unauthorized users are restricted.

Check file and directory details:
To inspect the current permissions, use the ls command with the -l option:
![image](https://github.com/aperezgomez/-Linux_file_permissions/assets/120771676/e61d1a78-44e7-4156-b75f-a7e16a09af84)

Describe the permissions string:
The permissions string in Linux is divided into four sections:

File type (d for directories, - for regular files)
Next three characters for user permissions.
Following three characters for group permissions.
Last three characters for other users' permissions.
For instance, a permission string of -rwxr-xr-- means:

Regular file (- at the start).
The user (owner) can read (r), write (w), and execute (x) the file.
The group can read (r) and execute (x) the file.
Others can only read (r) the file.

Change file permissions:
For example, we don't want Other users to have write access on project_k.txt. We can restrict their access using the chmod command:
![image](https://github.com/aperezgomez/-Linux_file_permissions/assets/120771676/445b8278-f760-43a2-ad29-f96ea70b9f4d)


Similarly, to ensure that Other users don't have read access to project_r.txt and project_t.txt:
![image](https://github.com/aperezgomez/-Linux_file_permissions/assets/120771676/e4639d90-6546-4e9b-bfa0-d16eb55b2250)

Change file permissions on a hidden file:
Hidden files in Linux start with a dot (.). The same chmod command can be used to adjust permissions on these files as well.

For .project_x.txt if we want to remove write permissions for the Group:
![image](https://github.com/aperezgomez/-Linux_file_permissions/assets/120771676/ea6f4540-c18b-4fa9-a58c-44eb5d7ff8e0)

Change directory permissions:
Directories should be given execute permissions to allow users to list its contents.

If we want to give read and execute permissions to the Group for the drafts directory:
![image](https://github.com/aperezgomez/-Linux_file_permissions/assets/120771676/352d06f1-36ef-4ee8-b63c-8c9c69cbb7cb)

Summary:
Linux provides a robust system for managing file and directory permissions using the chmod command. In this project, we inspected and adjusted the permissions of files and a subdirectory in the /home/researcher2/projects directory to ensure only authorized access. Proper file permission management is crucial for maintaining a secure system and ensuring that sensitive data is protected from unauthorized access. Regularly checking and managing these permissions should be an integral part of system administration tasks.


