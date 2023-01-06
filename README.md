ENTRAR EM FASTBOOT:

```bash
adb reboot bootloader
```

DESABILITAR VERIFICAÇÃO VBMETA:

```bash
fastboot flash --disable-verity --disable-verification vbmeta vbmeta.img
```

Entrar em FASTBOOTD:

```bash
fastboot reboot fastboot
```

Instalação da ROM:

```bash
fastboot flash system 
```

ENTRAR EM MODO RECOVERY PARA LIMPAR DADOS:

```bash
fastboot reboot recovery
```

INSTALL TWRP:

```bash
fastboot boot 
```

CASO PRECISE DELETAR A PARTIÇÃO:
system = product
system_a = product_a
system_b = product_b

```bash
fastboot delete-logical-partition product
```

```bash
fastboot delete-logical-partition product_a
```

```bash
fastboot delete-logical-partition product_b
```
