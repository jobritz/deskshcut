# deskshcut
create runnable Desktop shortcut in Kali Linux

# This Repository is about how you turn a command line you write in terminal into a one-click shortcut

# Step 1:
# create .sh file
# Write the command line you need to start the programm:
# Example: Xampp

sudo /opt/lampp/manager-linus-x64.run

# save this as an .sh file at a save place
# Step 2:
# add tag to make file runnable

chmod +x /where you saved your .sh file/filname.sh

# Step 3:
# create .desktop file:
# Disclaimer: Watch raw file to see the correct format

[Desktop Entry]
Version=1.0
Exec=/destination of your sh file/filname.sh
Name= --Anything--
GenericName= --Anything--
Comment= --Anything--
Encoding=UTF-8
Terminal=true
Type=Application
Categories=Application

# save this file anywhere now, you need to move it with terminal
# add tag to make file runable

chmod +x /where you saved your .dektop file/filename.desktop

# Step 4:
# move .desktop file:

sudo mv /where you saved your .desktop file/fileame. desktop /usr/share/applications

# Now you should be able to find this shortcut in your Applications
