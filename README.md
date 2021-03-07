# pyqgis_kernel

https://earthexplorer.usgs.gov/order/trackbulk/orderNum/1070782


How to create a pyqgis kernel in Jupyter-Notebook

1) Install the qgis kernal in terminal

2) Install the qgis in a jupyter-notebook

3) Using cmake to build a spatial library, then install to /opt/conda

git clone geospatial_project

cd geospatial_project

mkdir build

cd build

cmake -DCMAKE_INSTALL_PREFIX=/opt/conda ..

make -j 4



