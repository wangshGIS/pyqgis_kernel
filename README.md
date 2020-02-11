# pyqgis_kernel

How to create a pyqgis kernel in Jupyter-Notebook

1) Install the qgis kernal in terminal

#create qgis_stable kernel
conda create -y --name qgis_stable

#activate qgis_stable
conda activate qgis_stable

#install qgis
conda install -y -c conda-forge qgis

#install ipykernel
conda install -y -c anaconda ipykernel

#install qgis_stable in Jupiter-notebook

/opt/conda/envs/qgis_stable/bin/python -m ipykernel install --user --name "qgis_stable" --display-name "qgis_stable"


2) Config the pyqgis path in a  jupyter-Notebook

Create a jupyter Notebook

import sys
sys.path

sys.path.append('/opt/conda/envs/qgis_stable/share/qgis/python/plugins')
sys.path.append('/opt/conda/envs/qgis_stable/share/qgis/python')
sys.path.append('/opt/conda/envs/qgis_stable/bin')

#Testing qgis
import qgis.core
