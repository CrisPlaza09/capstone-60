# PCB_EN

Proyecto KiCad 10 (capstone). Abrir `PCB_EN.kicad_pro`.

Las librerias propias estan dentro del repo (`libs/`) y se cargan con `${KIPRJMOD}`,
asi que no hay que configurar nada. Los modelos 3D estandar usan `${KICAD10_3DMODEL_DIR}`
(KiCad 10 los instala por defecto).

- `libs/footprints/` footprints propios (`.pretty`)
- `libs/symbols/` simbolos propios (`.kicad_sym`)
- `libs/3d/` modelos 3D propios
- `fab/` Gerbers y taladros de la ultima exportacion
