# Spatial Analysis Tutorials

Welcome to the spatial analysis tutorials! This section contains both beginner and advanced materials.

## Beginner Tutorials
Start here if you're new to spatial analysis:

1. [**SpatialData Objects**](beginner/nb1_spatialdata_objects.ipynb): Introduction to working with spatial data structures
2. [**Static Plotting**](beginner/nb2_static_plotting.ipynb): Learn how to create static visualizations
3. [**Interactive Plotting with Napari**](beginner/nb3_interactive_plotting_with_napari.ipynb): Explore interactive visualization using Napari
4. [**Simple Analysis using scverse tools**](beginner/nb4_simple_analysis_using_scverse_tools.ipynb): Basic analysis techniques using the scverse toolkit

## Advanced Tutorials
Once you're comfortable with the basics, explore these more complex topics:

1. [**Transformations**](advanced/transformations.ipynb): Learn about spatial transformations and coordinate systems
2. [**Niche Calculation Tutorial**](advanced/tutorial_niche_calculation.ipynb): Advanced analysis of spatial niches and microenvironments

These advanced tutorials assume familiarity with the concepts covered in the beginner section.

## Environment setup instructions
In order to work with `SpatialData`, we will need to install some more packages. To avoid installation conflicts, we suggest to create a new environment, very similar to what was required for the first day.

```
conda create -y --name workshop_2025_spatial python=3.12
conda activate workshop_2025_spatial
pip install jupyterlab notebook
pip install spatialdata spatialdata-io spatialdata-plot napari-spatialdata squidpy pyproj
conda install -y ipykernel
python -m ipykernel install --user --name workshop_2025_spatial
```

We will use this environment throughout the afternoon.

## Data
We will work with publicly available data throughout the workshop:
- [10X Genomics datasets](https://www.10xgenomics.com/datasets?configure%5BhitsPerPage%5D=50&configure%5BmaxValuesPerFacet%5D=1000&refinementList%5Bplatform%5D%5B0%5D=Visium%20Spatial&refinementList%5Bplatform%5D%5B1%5D=Xenium%20In%20Situ&page=4) (hosts raw that that can be converted with `spatialdata-io`)
- [SpatialData-DB](https://lamin.ai/scverse/spatialdata-db/artifacts?filter[and][0][or][0][_branch_code][eq]=1&filter[and][1][or][0][is_latest][eq]=true) (hosts already converted `SpatialData` objects)
  - An example of how to work with the `SpatialData-DB` can be found [here](https://github.com/scverse/202503_hackathon_owkin/blob/main/data/template_notebook.ipynb).

## References
- [SpatialData documentation](https://spatialdata.scverse.org/en/latest/)
- [SpatialData-io documentation](https://spatialdata.scverse.org/projects/io/en/latest/)
- [SpatialData-plot documentation](https://spatialdata.scverse.org/projects/plot/en/latest/)
- [napari-SpatialData documentation](https://spatialdata.scverse.org/projects/napari/en/latest/)
- [Squidpy documentation](https://squidpy.readthedocs.io/en/stable/)
