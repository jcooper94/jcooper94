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
   ExecStart=/path/to/myscript.py
   Restart=always
   User=your_username
   Group=your_groupname

   [Install]
   WantedBy=multi-user.target
   ```

   Replace `/path/to/myscript.py` with the actual path to your Python script, and set the correct `User` and `Group`.

4. **Enable and start the service:**
   Run the following commands to enable and start the service:

   ```bash
   sudo systemctl enable myscript.service
   sudo systemctl start myscript.service
   ```

   This will ensure that your Python script starts automatically on boot and is restarted if it ever exits.

5. **Check the status:**
   You can check the status of your service with:

   ```bash
   sudo systemctl status myscript.service
   ```

```markdown
I had to add the following under `service`:

```
[Service]
ExecStart=/usr/bin/python3 /mnt/thevault/ui/homelabui/app.py
WorkingDirectory=/mnt/thevault/ui/homelabui
```

Then, to get it to run, I executed the following commands:

```bash
sudo systemctl daemon-reload
sudo systemctl enable your_service.service
sudo systemctl start your_service.service
```