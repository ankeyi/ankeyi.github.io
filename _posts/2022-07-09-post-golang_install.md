## golang env install
open linker <https://go.dev/dl/>
select  stable versions go1.18.3
my system os is archlinux-amd, select <b>go1.18.3.linux-amd64.tar.gz<b> download, or

	wget https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz   
	//save the file, move to /usr/local/go1.18.3.linux-amd64.tar.gz
```bash
	sudo tar zxvf go1.18.3.linux-amd64.tar.gz
	sudo mv go/  /usr/local/
	# write PATH=$PATH:/usr/local/go/bin to  /etc/profile
	sudo vim /etc/profile
		PATH=$PATH:/usr/local/go/bin
	# save && exit /etc/profile
	reboot
```		
