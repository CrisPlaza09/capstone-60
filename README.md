# PCB_EN (capstone 60%)

Proyecto KiCad 10. Todo lo necesario viene dentro del repo: no hay que instalar
ni configurar librerias.

## Como abrirlo

1. Descargar el repo: boton verde **Code → Download ZIP** (y descomprimir la carpeta completa)
   o `git clone https://github.com/CrisPlaza09/capstone-60.git`.
2. Abrir `PCB_EN.kicad_pro` con **KiCad 10**.

No mover ni borrar archivos sueltos: `fp-lib-table`, `sym-lib-table` y la carpeta `libs/`
deben quedar junto a `PCB_EN.kicad_pro`.

## Contenido

- `PCB_EN.kicad_pro / .kicad_sch / .kicad_pcb`: proyecto, esquematico y PCB
- `libs/footprints/`: footprints propios (`.pretty`)
- `libs/symbols/`: simbolos propios (`.kicad_sym`)
- `libs/3d/`: modelos 3D propios
- `fab/`: Gerbers y taladros de la ultima exportacion

## Notas tecnicas

- Las librerias propias se cargan con rutas relativas (`${KIPRJMOD}`), asi que funciona
  en cualquier PC y sistema operativo.
- Los modelos 3D estandar usan `${KICAD10_3DMODEL_DIR}`, que KiCad 10 define al instalarse.
  Con otra version mayor de KiCad pueden no verse en el visor 3D.
- Si se agrega un footprint o simbolo propio nuevo, guardarlo dentro de `libs/` y
  registrarlo en *Preferences → Manage Libraries → Project Specific Libraries*
  con ruta `${KIPRJMOD}/libs/...` (nunca con una ruta tipo `C:\...` o `D:\...`).
