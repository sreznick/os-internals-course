
## QEMU

[GitHub](https://github.com/qemu/qemu) 

Можно собирать независимо от toolchain.

1. Там нет официальных пререквизитов. Но мой опыт показывает, что надо установить следующее: 

```
sudo apt-get install -y pkg-config
sudo apt-get install -y libglib2.0-dev
sudo apt-get install -y libpixman-1-dev
```


2. ```git clone https://github.com/qemu/qemu```

3. ```cd qemu```

4. Конфигурируем и собираем

```
./configure --target-list=riscv64-softmmu
make
sudo make install
```

```make``` - без ```sudo```


