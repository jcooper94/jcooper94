If your feeling lazy you can change the default path where WSL2 starts your terminal, by using the following script I wrote. Simply change to the desired startup directory and use the provided `curl` command:

```bash
curl -o startup-script.sh https://raw.githubusercontent.com/jcooper94/Shell-Scripts/main/Bash/wsl2_startup.sh
```
Once you have the script, make it executable:
```bash
chmod +x startup-script.sh
```
Then run the script
```bash
./startup-script.sh
```

NOTE - Your C: filesystem is located as a mount point located at /mnt/c/, you probably want to make your home something like /mnt/c/users/<your username>/Documents or some other folder.

## Changing Default Path On Startup in WSL2 Terminal

To change the default path where WSL2 starts your terminal, you can modify the default shell profile settings. Here's how you can do it:

### For Ubuntu or Debian-based WSL2 distributions:

1. Open the terminal in WSL2.

2. Navigate to your home directory. You can use the `cd` command:

    ```bash
    cd ~
    ```

3. Open the `.bashrc` file in a text editor. You can use `nano`, `vim`, or any other editor you prefer:

    ```bash
    nano .bashrc
    ```

4. Add the following line at the end of the file to change the default directory:

    ```bash
    cd /desired/path
    ```

    Replace `/desired/path` with the actual path you want to set as the default.

5. Save the changes and exit the text editor.

6. Restart your terminal or run:

    ```bash
    source .bashrc
    ```