# Cleaner
Una herramienta de línea de comandos para detectar &amp; elimine el malware "hostflow" de los complementos de Minecraft infectados.
DESCARGAR: https://github.com/daysukee/Cleaner/releases/download/untagged-911e1af24262c12bae6a/Cleaner.jar

## Instalación
Descárguelo y colóquelo en la carpeta raíz de su servidor (donde se encuentran archivos como bukkit.yml, etc.)

## Modo de uso

#### Modo de detección:
```
Inicie su servidor con Cleaner.jar

Use: java -jar HostflowMalwareRemover.jar

Si usa algún panel, tendrá que seleccionar la versión personalizada del servidor y luego seleccionar este jar.
```

Si dice que encontró complementos con malware, debe realizar el siguiente paso.

#### Modo removedor:

```
Inicie su servidor con Cleaner.jar and add -D"remover=true"

Use: java -D"remover=true" -jar Cleaner.jar

Si usa algún panel, tendrá que seleccionar la versión del servidor personalizado y luego seleccionar este jar,
ahora en su panel en parámetros agregar al inicio -D"remover=true"
(si no puede hacer eso, deberá ponerse en contacto con su proveedor de alojamiento y pedirle que agregue eso o ejecute esta herramienta por usted)
(o también puede descargar todos los complementos de su host y ejecutar la herramienta en su PC)
```

Cuando termine, todos los complementos limpios estarán en "plugins-clean" folder,
luego renombrar "plugins" carpeta a "plugins1" o algo (para fines de copia de seguridad en caso de que no elimine el malware correctamente)
y ahora puedes renombrar "plugins-clean" a "plugins"

NOTA: Podría romper algunos complementos que usan el actual [Javassist](https://github.com/jboss-javassist/javassist) libreria,
si lo hace, debe descargar nuevamente ese complemento de fuentes oficiales.

#### Bibliotecas utilizadas:
- [ASM &amp; ASM Tree](https://asm.ow2.io/)
