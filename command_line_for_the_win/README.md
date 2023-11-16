Command line for the win

By: Sylvain Kalache, co-founder at Holberton School
Weight: 1
Date: Started Nov, 6, 2023
My name is: Victor Ukpongette

This project is a CMD game challenge, to refresh my knowlege on Bash command line skills


STEPS I USED IN UPLOADING MY SCREENSHOT FROM MY LOCAL MACHINE USING SFTP:

** I first completed the first 9 questions and took a screenshot then renamed it '0-first_9_tasks.png' and saved to my Desktop.
** I connected my sand box to my windows 10 CMD by coping the SFTP hostname and password as directed.
** I navigated with Bash commands to the directory 'command-line-for-the-win'.
** I used the command 'put C:\Users\wizzard\Desktop\0-first_9_tasks.png'(wizzard is my windows username)
** It was unsuccesful with the message 'stat wizzard/Desktop/0-first_9_tasks.png: No such file or directory'.
** I got confused and tried several times then discovered that the file name is automatically saved with and extension (.png) giving it the name '0-first_9_tasks.png.png' when i open the picture.
** I renamed the file from '0-first_9_tasks.png' to '0-first_9_tasks', giving it the freedom to automatically add the .png by itself.
** I came back and ran the command 'put C:\Users\wizzard\Desktop\0-first_9_tasks.png' again and it was successful.
** I displayed the directory content with command 'ls' to be sure, and i found it.
** I opened my sandbox webterm from my intranet and navigated to the project directory and found the file '0-first_9_tasks.png' there.
** I used the commands 'git add .', 'git commit' and 'git push' to upload to my github
