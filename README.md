Making Updates for Tech Policy Bruv
1. After changes to the code is made, push the changes to the github repository
2. Log in to the server via ssh
3. Enter the command "cd /var/www/techpolicybruv" to enter into the project directory
4. Pull the changes from the repository
5. Run the commands "sudo nginx -t" to check for errors and "sudo systemctl reload nginx" to reload the server and apply changes

To make changes to the site configurations on the server:
1. log in to the server via ssh
2. Enter the command "sudo nano /etc/nginx/sites-available/techpolicybruv" to open the configuration file
3. After changes are made, run the commands "sudo nginx -t" to check for errors and "sudo systemctl reload nginx" to reload the server and apply changes

How to log in to the server via ssh
1. Log in to ionos and go to the servers tab/page
2. Click on the respective server
3. Copy the IP address of the server i.e 212.345.67.60
4. On your mac terminal, enter the command "ssh root@{the copied ip address}"
5. This command will require a password, go back to the servers page/tab and copy the password from there
6. Paste the password in the terminal and press Enter.
