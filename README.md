# udacity-linuxserver

## Accessability

```
IP-address: 18.197.54.179
SSH Port: 2200
Connect: ssh -i key  grader@18.197.54.179 -p 2200
```

## Hosted web application

```
URL: http://ec2-18-197-54-179.eu-central-1.compute.amazonaws.com/
```

## Software and configuration changes

1. Started an instance with lightsail
2. Updated source list and removed unnecessary apps with update, upgrade and autoremove
3. Made changes to ufw and sshd_config to deny and allow ports
4. Disabled password based logins through sshd_config
5. Disabled root login through sshd_config
6. Created key-pair with ssh-keygen and gave the pubkey to grader user
7. Gave grader user sudo with the following command: sudo usermod -a -G sudo <name>
8. Updated timezone (sudo dpkg-reconfigure tzdata)
9. Installed Apache, mod_wsgi
10. Installed Git and cloned Catalog app from Github
11. Created a virtual environment to host dependencies, and installed them
12. Created a virtual host conifg file (/etc/apache2/sites-available/.conf)
13. Installed and configured postgresql
  a. Created user and table
  b. Gave user rights
  c. Updated python files from sqlite to postgresql (user: andy, pw: grader123)
14. Updated OAuth authorized JavaScript origins to make login work
15. Restarted Apache

## Third party resources

[Digital Ocean - Flask Deployment](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps)
