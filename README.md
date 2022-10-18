# Magikarp-Ground-Mission

PicoCTF picoGym Practice Challenges | Magikarp Ground Mission

![Thumbnail](https://user-images.githubusercontent.com/111799231/196515672-49dac90e-216d-4a57-aed0-f39d10d58943.jpg)

>Bored to read all the text? Well I can read it for you. Go to my Medium link (
https://medium.com/@theakaneasahi/picoctf-picogym-practice-challenges-magikarp-ground-mission-93ea5df624f3 ) and there is options that will read all these below texts for you.  

**What**  
```
picoCTF{xxsh_0ut_0f_\/\/4t3r_71be5264}  
```

**How**  
Start the instance. Then it will show you the ssh command to connect to this remote server. just copy paste it to your webshell. It will ask you if you really want to connect, so say yes say yes cuz I need to know.. You say I'll never get your blessin' 'til the day I die
"Tough luck, my friend, but the answer is no..
Oh wait. It's not saying no; it's actually asking for password. You will find the password on the problem. copy paste it and you are in!
Hey, you know what this whole writing is making boring as hell. I'm just giving my screenshots and snap of my work. Bon Appétit.
<img width="670" alt="flag" src="https://user-images.githubusercontent.com/111799231/196515709-f6dd79b9-aed9-40c0-9480-31af60482b59.png">

```
akane_asahi-picoctf@webshell:~$ ssh ctf-player@venus.picoctf.net -p 60407
The authenticity of host '[venus.picoctf.net]:60407 ([3.131.124.143]:60407)' can't be established.
ED25519 key fingerprint is SHA256:P1f6h95BrSVnJbm2AKhphfHHGEyAeThib/rN/AwKs24.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[venus.picoctf.net]:60407' (ED25519) to the list of known hosts.
ctf-player@venus.picoctf.net's password: 
Welcome to Ubuntu 18.04.5 LTS (GNU/Linux 5.4.0-1041-aws x86_64)
* Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage
This system has been minimized by removing packages and content that are
not required on a system that users do not log into.
To restore this content, you can run the 'unminimize' command.
The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.
Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.
ctf-player@pico-chall$ ls
1of3.flag.txt  instructions-to-2of3.txt
ctf-player@pico-chall$ cat 1of3.flag.txt 
picoCTF{xxsh_
ctf-player@pico-chall$ cat
^C
ctf-player@pico-chall$ cat instructions-to-2of3.txt 
Next, go to the root of all things, more succinctly `/`
ctf-player@pico-chall$ /
-bash: /: Is a directory
ctf-player@pico-chall$ ls
1of3.flag.txt  instructions-to-2of3.txt
ctf-player@pico-chall$ /..
-bash: /..: Is a directory
ctf-player@pico-chall$ ls
1of3.flag.txt  instructions-to-2of3.txt
ctf-player@pico-chall$ cd ..
ctf-player@pico-chall$ ls
3of3.flag.txt  drop-in
ctf-player@pico-chall$ cat 3of3.flag.txt 
71be5264}
ctf-player@pico-chall$ pwd
/home/ctf-player
ctf-player@pico-chall$ cd
ctf-player@pico-chall$ ls
3of3.flag.txt  drop-in
ctf-player@pico-chall$ cd..
-bash: cd..: command not found
ctf-player@pico-chall$ cd /
ctf-player@pico-chall$ ls
2of3.flag.txt  bin  boot  dev  etc  home  instructions-to-3of3.txt  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
ctf-player@pico-chall$ pwd
/
ctf-player@pico-chall$ cat instructions-to-3of3.txt 
Lastly, ctf-player, go home... more succinctly `~`
ctf-player@pico-chall$ ls 
2of3.flag.txt  bin  boot  dev  etc  home  instructions-to-3of3.txt  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
ctf-player@pico-chall$ cat 2of3.flag.txt 
0ut_0f_\/\/4t3r_  
```
**Why?**  
Let you understand how to connect to ssh and those 3 important commands to change directories.
