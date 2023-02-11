# BIODATACR
BIODATACR es una plataforma para la sistematización, documentación y publicación de información sobre la biodiversidad de Costa Rica.

## Ambientes Conda
Estos ambientes se emplean para el desarrollo de aplicaciones en varios lenguajes de programación.

### R

**Creación**
```shell
# Creación de un ambiente Conda para R
conda update conda -y
conda create -y -n biodatacr-r
conda activate biodatacr-r
conda config --env --add channels conda-forge
conda config --env --set channel_priority strict
conda install -y mamba
mamba install -y r-base r-essentials r-vroom=1.5.7 r-ggthemes r-hrbrthemes r-plotly r-dt r-sf=1.0_6 r-leaflet r-rgbif
```

**Borrado**
```shell
# Borrado del ambiente Conda
conda deactivate
conda env remove --name biodatacr-r
```
