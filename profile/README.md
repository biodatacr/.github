# BIODATACR

## Ambientes Conda

### R

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

# Borrado del ambiente Conda
```shell
conda deactivate
conda env remove --name biodatacr-r
```
