# Assembly
# To set up in Ubuntu 20.04+
# Install Doxbox  
sudo apt update && sudo apt install dosbox -y
dosbox 

# Inside dosbox (give it some path in your host machine) 
# Put extracted contents of the zip file and .asm files in this folder on your host machine 

mount c /home/yourusername/nasm 

c: 

# Assemble and run 
nasm c.asm -o c.com 
afd c.com 

# Assemble with Listing 
nasm c.asm -l c.lst -o c.com 

# If after changing files, they do not show up in dosbox, hit Ctrl+F4 inside the dosbox window. 
