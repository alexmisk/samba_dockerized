# Dockerized Samba
Generic samba docker-compose file for easy file sharing

## Installation & usage
1. Clone the repo:
```
git clone https://github.com/alexmisk/samba_dockerized.git
```

2. Change to the repo's dir and rename the example file:  
```
cd samba_dockerized && mv samba.env.example samba.env
```

3. Edit `USER` and `SHARE` environmental variables for you needs:
```
USER=<your_username>;<your_password>

...

SHARE=<share_name>;/mnt;yes;no;no;<your_username>;'none';'none'
```

4. Start the service via docker-compose:
```
docker-compose up -d
```

5. Login to the share via SMB protocol
