========================================================
Creating custom applications built on QGIS libraries
========================================================

It is better to run some processes automatically than manually.
On our courses, we try to promote this approach.
While working with geospatial data in Fiona, RasterIO or GDAL formats, it is no surprise that we can also use QGIS libraries.

Base module is qgis.core, which is required by various tasks that process data.
With QGIS libraries, you can also create your own application with graphical interface.
This can be achieved by using module `qgis.gui`, which enables many interesting options such as *canvas*, which we can use to display maps and so on.

Base structure of project
------------------------

Before we start using QGIS libraries, we need to configure some settings for the start and the end of our script. 


.. literalinclude:: ../scripts/standalone.py
   :language: python
   :linenos:

After setting up permissions to *launch file* `chmod 755 standalone.py` we can safely launch it and leave it running.

.. note:: It is possible that you will need to set up correct variable
    :envvar:`PYTHONPATH` with path to Python libraries for QGIS.

.. _fiona: https://fiona.readthedocs.io/en/stable/
.. _rasterio:  https://rasterio.readthedocs.io/en/latest/
.. _gdal: https://pcjericks.github.io/py-gdalogr-cookbook/
