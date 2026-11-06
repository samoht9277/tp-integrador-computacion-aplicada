# TP Integrador — Computación Aplicada

Universidad de Palermo · Profesor: Matias Chiesa · 2026

## Integrantes

- Tomás CASAGRANDE
- Cristian Nehuen APABLAZA ORTEGA

## ¿Qué hay en este repositorio?

Copias comprimidas de los directorios del servidor **TPServer** (Debian 12), tal como quedaron después de resolver el TP:

| Archivo | Qué contiene |
|---|---|
| `root.tar.gz` | `/root`, el directorio personal de root |
| `etc.tar.gz` | `/etc`, la configuración del sistema |
| `opt.tar.gz` | `/opt`, con el script de backup y el archivo `particion` |
| `www_dir.tar.gz` | `/www_dir`, la página web (`index.php` y `logo.png`) |
| `backup_dir.tar.gz` | `/backup_dir`, los backups generados |
| `var.tar.gz.part-aa` a `var.tar.gz.part-ad` | `/var`, dividido en 4 partes de 10 MB |

## ¿Cómo abrir los archivos?

Cada `.tar.gz` se descomprime así:

```sh
tar -xzf root.tar.gz
```

`/var` está dividido en partes. Primero hay que unirlas y después descomprimir:

```sh
cat var.tar.gz.part-* > var.tar.gz
tar -xzf var.tar.gz
```
