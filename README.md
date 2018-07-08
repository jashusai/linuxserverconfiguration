# linuxserverconfiguration
# About:

This is the 6th project in udacity about the linux server.

# Details of my server:

13.127.33.67.xip.io

# Url site:

https://13.127.33.67.xip.io/

# Password of grader:

jash

# Latest version to update:

sudo apt-get update

# Grader key:

-----BEGIN RSA PRIVATE KEY-----
MIIEpQIBAAKCAQEAySyqm+/Kr8/UB3SVoi5L68qjtQX3F0JKT9KtCZn1SxRXl+H2
+z9wg53+AAlWAuDyfqhU+NKwiyxQCS4L0glYkLGp8IXJXHhK4h/LJo5Bn0zIoEWH
F8clv8EDG43RmG8Z13PvL/3lb1S5yx5a4RZ/td4mnxsZQHxelyxld9EuIOv4xImQ
4PGK8ZrJn4hryoKZR+u3k9alxfOjH3/ym++SUFnpySu1NRqCf7+iJvsDo/uBiYHO
iXCXk0YFn5Nyex2XVfqonkDETxoeisJt6UI/hAyd0wHNupWnJK02Z0G3ES9yGLXY
y3nSw54EBM+SHayaM7d+J82C7vWRTETmBbiS4QIDAQABAoIBAQCXObVyjTpPGSqp
BBGrnaPCt0yCut44pMNZ5+PdsNc8vijuapWP3uuEdRLIEjyO42xGm+FsPm0p4YC0
teF63T2vX26A+QEaOu8HtqCu9gcMadry5/EahcCxubTNVLl3HiVN2b+20uRS4Vzc
/I+SXqhYHYvo1KUR3av5dg08mYlUgtkAbq+MeIrNuioUbsDHdGG6esOrptq5zJsH
SuCeQpKLqsNUg0z8DaepLPFRyYw2GyrDnHe5SHYqPngjFXBfXmzwZdybbpSikGzr
urZHVZ1eH3Gyx7czuSJ6dTNP5xmG91ruhWYPlq98T6Aikmwjls+8ATFQwmUw7ijp
C0mbQFvVAoGBAOYi4CsQyMihVKDdQpO587IQ9wlIRSutPg/bbgCG7PRBIcb0jrH2
j8+4jBynnoDRFcSegzgCf72Qac6Zpi5UlAQEC/i8S2SpedAWNwpFWpXBSICCf85k
RlaQpY4sZtKuE1rmARMVx+kpjE5jYpqIHdZvxfXWl91sNNcSp47hMqkTAoGBAN/I
jEL8cpKBYqGXscrqr6UIweFTpVs6AYl0pXtesan2j5IKyvOLT1TEFzbUr83N5YKO
+HBdu4Yh87yr3YDRwROUBA9MFAAy8Q5IxaQDSlVra8WL3S2ycKSxu+/EnUQVXgCK
3xwEQASI46wha4920kDyg43zSqPjRh6Y76SA8Oa7AoGAQRGnVEXgn2mOJhWpV1+C
WdyWHJfEhv7qx00Bo0CDCuTHihtnpUXTj6XcZ9W06TM09mzjKRj7yTtlzzZ+WCct
2pzSTbffkUyh1oYRdeP6ItGNkFhVjqOnh55KURKY2ATEEDVsJFtKNNC8jQVowcyu
swzTahkMw1xu7Ein+6wMyOUCgYEAkg9cdPA+e58VWDEhazboc4gWu1IUEEn47NWE
mNRCk5OJO6Htuy4HFmVyXWhOYr5reV6FixmypqaMZm2qgkTlhzjJuY5HU6XsLg2T
aix3nO8jBWn3b7cSzHvxFVq35tMnaqU5YBjqC8upBhU+FgJQ0vE2qjTMV9GkV54s
c6txELcCgYEAmc0OlHCft7hbUe6HeOuoD6bMsLtIfLoQ8KowavHHkYKWrGIWJDvm
YpW3yYtBjbrdchbVRXEunLgQxsEbL3OVsKm9KvQf2BAnAYhb+TkMbrjVT2AmnaA2
lTCD8P9woMTv6bwvNA18s/GqjvLXwDn4Fw29CARrd0h/7al8eTQexho=
-----END RSA PRIVATE KEY-----

## id_rsa.pub key:

ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDJLKqb78qvz9QHdJWiLkvryqO1BfcXQkpP0q0JmfVLFFeX4fb7P3CDnf4ACVYC4PJ+qFT40rCLLFAJLgvSCViQsanwhclceEriH8smjkGfTMigRYcXxyW/wQMbjdGYbxnXc+8v/eVvVLnLHlrhFn+13iafGxlAfF6XLGV30S4g6/jEiZDg8YrxmsmfiGvKgplH67eT1qXF86Mff/Kb75JQWenJK7U1GoJ/v6Im+wOj+4GJgc6JcJeTRgWfk3J7HZdV+qieQMRPGh6Kwm3pQj+EDJ3TAc26lackrTZnQbcRL3IYtdjLedLDngQEz5IdrJozt34nzYLu9ZFMROYFuJLh


#  connecting the grader:

ssh -i path/to/privatekey -p 2200 grader@13.127.33.67

# Creating grader user:

sudo adduser grader

# give permissions to new user:

sudo nano /etc/sudoers

# In the root user add the line:

grader ALL=(ALL:ALL) ALL => give sudo permissions to grader.

# For a grader to form a ssh key pair:
 
 ssh-keygen => generate a public and private ssh keys and saved to .ssh folder.
 
 # putty software:
 
 Generate a private keys with default file.
 
 Open virtual machine in putty and change to grader user:
 su - grader
 
 # Generate a new directory .ssh to authorized_keys:
 
  mkdir.ssh
  
  # create a file in that folder:
  
  sudo nano .ssh/authorized_keys => save the file with .pub extension to authorized_keys.
  
  # Give permissions to directory:
  
  chmod 700 .ssh
  
  chmod 644 .ssh/authorized_keys
  
  # Restart the ssh server:
  
  service ssh restart
  
  # port changing:
  
  ssh -i .ssh/id_rsa grader@13.127.33.67(in editor)
  sudo nano /etc/ssh/sshd_config
  
  restart the ssh server:
  service ssh restart
  
  # Login to grader:
  
  ssh -i .ssh/id_rsa grader@13.127.33.67
  
  # Disabling root as ssh login:
  
  sudo nano /etc/ssh/sshd_config
  
  # Preventing root:
  
  change PermitRootLogin preventing passwored to "no"
  
  #  Safety Firewall commands:
  
  sudo ufw default deny incoming 
  
  sudo ufw allow 2200/tcp

  sudo ufw allow 80/tcp

  sudo ufw allow 123/udp

  sudo ufw enable
  
  # Checking the status:
  
  sudo ufw status => allowing ports to display.
  
  # Apache2 installing:
  
  sudo apt-get install apache2
  
  # Mod_wsgi:
  
  sudo apt-get install python-setuptools libapache2-mod-wsgi
  
  # Enable mod_wsgi:
  
  sudo a2enmod wsgi
  
  # New directory creating:
  
  In /var/www directory create a new folder -> sudo mkdir FlaskApp
                                               cd FlaskApp
                                               
   # git installation:
   
   sudo apt-get install git
   
   # clone your github repository:
   
   sudo git clone https://github.com/username/catalog.git
   
   # changing the project file:
   
   __init__.py
   
   
  
  
  
 
 
 



