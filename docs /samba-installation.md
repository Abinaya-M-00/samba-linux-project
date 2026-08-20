# Samba Installation

# 1. Update Package Repository
sudo apt update

# 2. Install Samba
sudo apt install samba -y

# 3. Check Samba Service
sudo systemctl status smbd

# 4. Check Samba Version
smbd --version

# 5. Enable Samba at Boot
sudo systemctl enable smbd

# 6. Start Samba Service
sudo systemctl start smbd

# 7. Verify Samba Service
sudo systemctl status smbd
