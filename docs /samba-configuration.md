# Samba Configuration

# 1. Create Shared Directory
sudo mkdir -p /srv/samba/shared

# 2. Set Directory Permissions
sudo chmod 777 /srv/samba/shared


# 3. Edit Samba Configuration
sudo nano /etc/samba/smb.conf

Add the following configuration:

[shared]
   path = /srv/samba/shared
   browsable = yes
   read only = no
   guest ok = yes

# 4. Check Samba Configuration
testparm

# 5. Restart Samba Service
sudo systemctl restart smbd

# 6. Check Samba Service
sudo systemctl status smbd
