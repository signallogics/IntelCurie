# CODK-A

```sh
user@workstation:~/Intel/Curie$ mkdir -p ~/CODK && cd $_
```

```sh
user@workstation:~/CODK$ git clone https://github.com/01org/CODK-A.git
Clonar en «CODK-A»...
remote: Counting objects: 70, done.
remote: Total 70 (delta 0), reused 0 (delta 0), pack-reused 70
Unpacking objects: 100% (70/70), done.
Comprobando la conectividad… hecho.
user@workstation:~/CODK$ cd CODK-A/
user@workstation:~/CODK/CODK-A$ ls
LICENSE  Makefile  README.md
```

```sh
user@workstation:~/CODK/CODK-A$ make clone
git clone -b master https://github.com/01org/CODK-A-ARC.git /home/user/CODK/CODK-A//arc
Clonar en «/home/user/CODK/CODK-A//arc»...
remote: Counting objects: 164, done.
remote: Total 164 (delta 0), reused 0 (delta 0), pack-reused 163
Receiving objects: 100% (164/164), 2.34 MiB | 840.00 KiB/s, done.
Resolving deltas: 100% (58/58), done.
Comprobando la conectividad… hecho.
git clone -b master https://github.com/01org/CODK-A-X86.git /home/user/CODK/CODK-A//x86
Clonar en «/home/user/CODK/CODK-A//x86»...
remote: Counting objects: 7282, done.
remote: Total 7282 (delta 0), reused 0 (delta 0), pack-reused 7282
Receiving objects: 100% (7282/7282), 161.83 MiB | 958.00 KiB/s, done.
Resolving deltas: 100% (2837/2837), done.
Comprobando la conectividad… hecho.
Checking out files: 100% (8293/8293), done.
ln -s /home/user/CODK/CODK-A/x86 /home/user/CODK/CODK-A/firmware
git clone -b master https://github.com/01org/CODK-A-Bootloader.git /home/user/CODK/CODK-A//x86/bsp/bootable/bootloader
Clonar en «/home/user/CODK/CODK-A//x86/bsp/bootable/bootloader»...
remote: Counting objects: 145, done.
remote: Total 145 (delta 0), reused 0 (delta 0), pack-reused 145
Receiving objects: 100% (145/145), 253.71 KiB | 413.00 KiB/s, done.
Resolving deltas: 100% (33/33), done.
Comprobando la conectividad… hecho.
git clone -b master https://github.com/01org/CODK-A-Flashpack.git /home/user/CODK/CODK-A//flashpack
Clonar en «/home/user/CODK/CODK-A//flashpack»...
remote: Counting objects: 6576, done.
remote: Total 6576 (delta 0), reused 0 (delta 0), pack-reused 6576
Receiving objects: 100% (6576/6576), 20.68 MiB | 1.00 MiB/s, done.
Resolving deltas: 100% (1679/1679), done.
Comprobando la conectividad… hecho
user@workstation:~/CODK/CODK-A$ 
```

```sh
user@workstation:~/CODK/CODK-A$ sudo make install dep
sudo: imposible resolver el anfitrión workstation
make: *** No hay ninguna regla para construir el objetivo «install».  Alto.
pymelab@workstation:~/CODK/CODK-A$ 
```

```sh
user@workstation:~/CODK/CODK-A$ make compile-x86
user@workstation:~/CODK/CODK-A$ make compile-arc
user@workstation:~/CODK/CODK-A$ make compile
```

```sh
user@workstation:~/CODK/CODK-A$ make upload-x86
user@workstation:~/CODK/CODK-A$ make upload-arc
user@workstation:~/CODK/CODK-A$ make upload
```

