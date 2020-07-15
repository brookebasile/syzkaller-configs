Configs I used for installing syzkaller on a QEMU VM on my machine using (loosely) the following guide:
<https://www.collabora.com/news-and-blog/blog/2020/04/17/using-syzkaller-to-detect-programming-bugs-in-linux/>

Add this to ssh config (``~/.ssh/config``) to make it *a lot* easier to access the VM:
```
Host syzkaller
        Hostname localhost
        User root
        IdentityFile ~/.ssh/stretch.id_rsa
        Port 10021
        StrictHostKeyChecking no
```
