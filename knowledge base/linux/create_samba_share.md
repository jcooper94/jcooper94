```bash
# Install Samba (if not already installed)
sudo apt-get install samba

# Create a directory for your share
sudo mkdir /path/to/your/share

# Set appropriate permissions for the share
sudo chmod -R 0777 /path/to/your/share

# Configure Samba
sudo nano /etc/samba/smb.conf

# Add the following lines at the end of the file
[YourShareName]
  path = /path/to/your/share
  read only = no
  browsable = yes
  guest ok = yes

# Save and exit (Ctrl + X, Y, Enter)

# Restart Samba service
sudo service smbd restart

# Open /etc/fstab for editing
sudo nano /etc/fstab

# Add the following line at the end
//localhost/YourShareName /mnt/mountpoint cifs guest,uid=1000,iocharset=utf8 0 0

# Replace /mnt/mountpoint with your desired mount point

# Save and exit (Ctrl + X, Y, Enter)

# Test the configuration and mount the share
sudo mount -a
```