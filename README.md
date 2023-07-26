# Siesta Code
Spanish Initiative for Electronic Simulations with Thousands of Atoms

## Installation

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

# PASO INTERMEDIO:INSTALAR gfortran si no se tiene.

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
