# Samba Troubleshooting

# 1. Check Samba Service
sudo systemctl status smbd

# If the service is not running:
sudo systemctl restart smbd

# 2. Check Samba Configuration
testparm

# 3. Check Samba Port
sudo ss -tlnp | grep 445

# 4. Check Firewall
sudo ufw status

# If the firewall is active, allow Samba:
sudo ufw allow samba

# 5. Check Samba Logs
sudo journalctl -u smbd
