# linux-ammon
Linux empotrado para el monitor con el sensor AM2320

Los archivos generados siguen los parametros configurados en dos archivos:
  1 .config que se encuentra en la carpeta principal de buildroot y se configuró mediante el comando make xconfig
  2 .config que se encuantra en output/build/linux-1587f77/.config y se configuró mediante el comando make linux-menuconfig
  
De los archivos generados solo se hilan los sensibles a sufrir modificación. Los archivos de /output/images por los que la estructura de directorios del git es:
  
  .
  |
  output
   \images              #Archivos generados por buildroot al compilar
  | 
  configs
   \builroot\.config    #Archivo configuración de buildroot
   \linux\.config       #Archivo configuración del kernel
   
La versión usada de buildroot es la versión 2013.11 para la cual se ha usado u-boot 2013.
Se puede descargar builroot 2013.11 desde: https://buildroot.org/downloads/buildroot-2013.11.tar.gz
