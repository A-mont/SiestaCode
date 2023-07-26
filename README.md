# Siesta Code

## Descripción 
Spanish Initiative for Electronic Simulations with Thousands of Atoms

## Instalación

## PASO 1 DESCARGAR wget
**comando:**
```bash
apt-get install wget
```

## PASO 2 DESCARGAR SIESTA.tar

**comando:**
```bash
wget https://launchpad.net/siesta/4.1/4.1-b4/+download/siesta-4.1-b4.tar.gz
```

## PASO 3 DESCOMPRIMIR

**comando:**
```bash
tar -xvf siesta-4.1-b4.tar.gz
```

## PASO 4 ENTRAR A LA CARPETA SIESTA

**comando:**
```bash
cd siesta-4.1-b4/Obj
```

## PASO 5 EJECUTAR SCRIPT EN CARPETA OBJ

**comando:**
```bash
sh ../Src/obj_setup.sh
```

### PASO INTERMEDIO:INSTALAR gfortran si no se tiene.

**comando:**
```bash
sudo apt-get update
```
**comando:**
```bash
sudo apt-get install gfortran
```

## PASO 6 CREAR arch.make
**comando:**
```bash
cp gfortran.make arch.make
```

## PASO 7 CREAR EL EJECUTABLE DE SIESTA

**comando:**
```bash
make
```

## PASO 8 VERIFICAR EL CORRECTO FUNCIONAMIENTO DEL EJECUTABLE

**comando:**
```bash
./siesta
```

## Hola mundo con Siesta

## Paso 1 CREAMOS EL DIRECTORIO H2
**comando:**
```bash
mkdir H2
```
## Paso 2 DESCARGAMOS EL TUTORIAL
```bash
cd H2
wget https://personales.unican.es/junqueraj/JavierJunquera_files/Metodos/Basic/H2/Files-h2.tar
```
## Paso 3 DESCOMPRIMIMOS
**comando:**
```bash
tar -xvf Files-h2.tar
```
## Paso 4 COPIAMOS EL EJECUTABLE DE SIESTA EN /Obj
**comando:**
```bash
cp ../siesta-4.1-b4/Obj/siesta .
```
## Paso 4 USAMOS EL EJECUTABLE DE SIESTA CON EL ARCHIVO DE ENTRADA .FDF GENERANDO UN .OUTPUT COMO SALIDA.
**comando:**
```bash
./siesta <h2.fdf > H.output
```
## Paso 5 EL RESULTADO GENERARÁ LOS SIGUIENTES DIRECTORIOS:
**comando:**
```bash
0_NORMAL_EXIT          CLOCK         H.ion      H.psf            MESSAGES             PARALLEL_DIST  fdf-63183.log   h2.DM   h2.KP          h2.XV   siesta
BASIS_ENTHALPY         FORCE_STRESS  H.ion.xml  INPUT_TMP.24403  NON_TRIMMED_KP_LIST  README         h2.BONDS        h2.EIG  h2.ORB_INDX    h2.bib  siesta.bib
BASIS_HARRIS_ENTHALPY  Files-h2.tar  H.output   INPUT_TMP.63161  OUTVARS.yml          fdf-24407.log  h2.BONDS_FINAL  h2.FA   h2.STRUCT_OUT  h2.fdf
```
