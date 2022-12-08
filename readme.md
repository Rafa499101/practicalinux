# Práctica Linux

##  Diciembre 2022

1- Set static ip on your Linux device to connect to your LAN using nmcli command.

*nmcli connection modify enp0s3 ipv4.address 192.168.6.30/24*

*nmcli connection modify enp0s3 ipv4.gateway 192.168.6.1*

*nmcli connection modify enp0s3 ipv4.dns 192.168.6.2*

*Disable network interface with nmcli*

![](/img\img01.PNG)

2- Disable the nmcli network interface

*nmcli connection down enp0s3*

3-  Activate the nmcli network interface

*nmcli connection up enp0s3*

![](/img\img02.PNG)

4- Check with the ip command your configuration

![](/img\img03.PNG)

5-  Do ping to nodes on your network

*ping 192.168.6.5*

![](/img\img04.PNG)

6-  Lists all .txt files in the current directory and then counts those .txt files and saves the output to a new  file.

*ls *.txt | wc -l > count.txt*

![](/img\img05.PNG)

7- Create a file from scratch on linux and include the following information

*$ cat - >> newfile.txt this is the file create in linux with some information will be copied to another host in the network ^Z $*

![](/img\img06.PNG)

8- Copy it from another host on your network

*scp p03.txt root@192.168.6.30.*

![](/img\img07.PNG)

9- Connect to the other host and verify that it has been created.

*ssh root@192.168.6.30*

*ls -l*

![](/img\img08.PNG)

10-  Download from ubuntu website page the iso with wget command and curl command.

*wget http://releases.ubuntu.com/focal/ubuntu-20.04.5-desktop-amd64.iso*

![](/img\img09.PNG)

11- Download SHA256 files and confirm that the downloaded file is correct (SHA256SUM) from the same  page.