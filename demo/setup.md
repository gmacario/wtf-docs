# Setting up the WTF demo

* (optional) Connect serial console to UDOO NEO - See [here](http://gmacario.github.io/howto/udoo/neo/embedded/software/development/2015/11/08/connecting-to-udoo-neo-serial-console.html)
* TODO

Stop U-Boot, update U-Boot commandline

```
udoo_boot_init=if run loadbootscript; then run bootscript; fi; udooinit; ext2load mmc 0:5 ${fdt_loadaddr} ${fdt_file};
```

Change to

```
setenv udoo_boot_init "if run loadbootscript; then run bootscript; fi; udooinit; ext2load mmc 0:5 ${fdt_loadaddr} dts/imx6sx-udoo-neo-extended-lvds7-m4.dtb;"
saveenv
reset
```

<!-- EOF -->
