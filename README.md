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
8. Deployed a FlaskApp using ...


## List of third-party resources used in the project







Locate the SSH key you created for the grader user.

During the submission process, paste the contents of the grader user's SSH key into the "Notes to Reviewer" field.
