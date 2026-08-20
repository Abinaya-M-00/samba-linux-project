# Samba Commands

# Check Samba Installation
samba --version

# Install Samba
sudo apt update
sudo apt install samba -y

# Check Samba Service
sudo systemctl status smbd

# Start Samba
sudo systemctl start smbd

# Enable Samba at Boot
sudo systemctl enable smbd

# Restart Samba
sudo systemctl restart smbd

# Check Configuration
testparm
