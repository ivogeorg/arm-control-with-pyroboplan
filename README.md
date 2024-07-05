```
user:~$ more course_install.sh
# Install dependencies of PyRoboPlan
cd pyroboplan
pip install -e .

# Install chrome (and remove firefox)
sudo apt update
wget -P ~/Downloads https://dl.google.com/linux/direct/google-ch
rome-stable_current_amd64.deb
sudo apt install -y libu2f-udev xdg-utils
sudo dpkg -i ~/Downloads/google-chrome-stable_current_amd64.deb
sudo apt install -f
rm ~/Downloads/google-chrome-stable_current_amd64.deb

# Remove apt versions of matplotlib and firefox
sudo apt remove -y firefox python3-matplotlib

echo -e "\nInstallation complete!\n"
```
