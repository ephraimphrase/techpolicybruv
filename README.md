Move to local repo
1. Click on Code
2. Under HTTPS, copy the URL
3. In your local development environment (like VSCode), endter the following in the termnal: "git clone *the copied URL*"
4. After making the changes, push to the github repo, (git add ., git commit -m "message", git push origin master)

Making Updates for Tech Policy Bruv
1. Open terminal app
2. Log in to ionos and go to the servers tab/page
3. Click on the respective server
4. Copy the IP address of the server (Host) i.e 212.345.67.60
5. On your mac terminal, enter the command "ssh root@{the copied ip address}". This command will require a password
6. Go back to the servers page/tab and copy the password
7. Paste the password in the terminal and press Enter.
8. Enter the command "cd /var/www/techpolicybruv" to enter into the project directory
5. Pull the changes from the repository by entering the command: "git pull origin master"
6. Run the commands "sudo nginx -t" to check for errors and "sudo systemctl reload nginx" to reload the server and apply changes

To make changes to the site configuration file on the server:
1. log in to the server via ssh
2. Enter the command "sudo nano /etc/nginx/sites-available/techpolicybruv" to open the configuration file 
3. After changes are made, run the commands "sudo nginx -t" to check for errors and "sudo systemctl reload nginx" to reload the server and apply changes
4. The commands to exit or save are listed at the bottom of the terminal window... to exit ^x (Control + x)
