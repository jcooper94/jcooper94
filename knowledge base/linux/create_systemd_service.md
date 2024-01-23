Here's the corrected markdown formatting for your content:

1. **Create a Python script:**
   Create your Python script, for example, `myscript.py`. Make sure it has the necessary shebang at the beginning:

   ```python
   #!/usr/bin/env python3

   # Your Python code here
   ```

2. **Make the script executable:**
   Open a terminal and navigate to the directory containing your script. Make the script executable with the following command:

   ```bash
   chmod +x myscript.py
   ```

3. **Create a systemd service unit:**
   Create a systemd service unit file, e.g., `myscript.service`, in the `/etc/systemd/system/` directory. Open the file in a text editor and add the following content:

   ```ini
   [Unit]
   Description=My Python Script

   [Service]
   ExecStart=/usr/bin/python3 /your/location/app.py
   WorkingDirectory=/your/location/
   Restart=always
   User=your_username
   Group=your_groupname

   [Install]
   WantedBy=multi-user.target
   ```

4. **Enable and start the service:**
   Run the following commands to enable and start the service:

   ```bash
   sudo systemctl daemon-reload   # Add this line
   sudo systemctl enable myscript.service
   sudo systemctl start myscript.service
   ```

   This will ensure that your Python script starts automatically on boot and is restarted if it ever exits.

5. **Check the status:**
   You can check the status of your service with:

   ```bash
   sudo systemctl status myscript.service
   ```