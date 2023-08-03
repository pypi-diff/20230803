# Comparing `tmp/hydromt_sfincs-1.0.0.tar.gz` & `tmp/hydromt_sfincs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydromt_sfincs-1.0.0.tar", last modified: Mon Apr 17 16:01:50 2023, max compression
+gzip compressed data, was "hydromt_sfincs-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hydromt_sfincs-1.0.0.tar` & `hydromt_sfincs-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,31 @@
--rw-r--r--   0        0        0     1380 2023-04-17 16:01:40.052248 hydromt_sfincs-1.0.0/.gitignore
--rw-r--r--   0        0        0      819 2023-04-17 16:01:40.052248 hydromt_sfincs-1.0.0/.zenodo.json
--rw-r--r--   0        0        0    35148 2023-04-17 16:01:40.052248 hydromt_sfincs-1.0.0/LICENSE
--rw-r--r--   0        0        0     5339 2023-04-17 16:01:40.052248 hydromt_sfincs-1.0.0/README.rst
--rw-r--r--   0        0        0      535 2023-04-17 16:01:40.056248 hydromt_sfincs-1.0.0/environment.yml
--rw-r--r--   0        0        0      215 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/__init__.py
--rw-r--r--   0        0        0      197 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/README
--rw-r--r--   0        0        0     1151 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/corine_mapping.csv
--rw-r--r--   0        0        0      335 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/esa_worldcover_mapping.csv
--rw-r--r--   0        0        0     1702 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/globcover_mapping.csv
--rw-r--r--   0        0        0      874 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/vito_mapping.csv
--rw-r--r--   0        0        0      658 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/data/sfincs/sfincs.inp
--rw-r--r--   0        0        0    10523 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/plots.py
--rw-r--r--   0        0        0    21886 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/regulargrid.py
--rw-r--r--   0        0        0   120821 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/sfincs.py
--rw-r--r--   0        0        0     6414 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/sfincs_input.py
--rw-r--r--   0        0        0    29380 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/subgrid.py
--rw-r--r--   0        0        0    25856 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/utils.py
--rw-r--r--   0        0        0      171 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/__init__.py
--rw-r--r--   0        0        0    15096 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/bathymetry.py
--rw-r--r--   0        0        0     3444 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/discharge.py
--rw-r--r--   0        0        0     5285 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/flwdir.py
--rw-r--r--   0        0        0      630 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/landuse.py
--rw-r--r--   0        0        0    10030 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/merge.py
--rw-r--r--   0        0        0    12754 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/tiling.py
--rw-r--r--   0        0        0     1911 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7038 1970-01-01 00:00:00.000000 hydromt_sfincs-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1380 2023-08-03 16:01:19.537177 hydromt_sfincs-1.0.1/.gitignore
+-rw-r--r--   0        0        0      852 2023-08-03 16:01:19.537177 hydromt_sfincs-1.0.1/.zenodo.json
+-rw-r--r--   0        0        0    35148 2023-08-03 16:01:19.541178 hydromt_sfincs-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5261 2023-08-03 16:01:19.541178 hydromt_sfincs-1.0.1/README.rst
+-rw-r--r--   0        0        0      535 2023-08-03 16:01:19.541178 hydromt_sfincs-1.0.1/environment.yml
+-rw-r--r--   0        0        0      215 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/__init__.py
+-rw-r--r--   0        0        0      718 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/data/lulc/NLCD_HSG.csv
+-rw-r--r--   0        0        0      461 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/data/lulc/NLCD_SFBD_mapping.csv
+-rw-r--r--   0        0        0      197 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/data/lulc/README
+-rw-r--r--   0        0        0     1151 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/data/lulc/corine_mapping.csv
+-rw-r--r--   0        0        0      334 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/data/lulc/esa_worldcover_HSG.csv
+-rw-r--r--   0        0        0      335 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/data/lulc/esa_worldcover_mapping.csv
+-rw-r--r--   0        0        0     1702 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/data/lulc/globcover_mapping.csv
+-rw-r--r--   0        0        0      874 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/data/lulc/vito_mapping.csv
+-rw-r--r--   0        0        0      658 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/data/sfincs/sfincs.inp
+-rw-r--r--   0        0        0    11875 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/plots.py
+-rw-r--r--   0        0        0    21885 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/regulargrid.py
+-rw-r--r--   0        0        0   148185 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/sfincs.py
+-rw-r--r--   0        0        0     6413 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/sfincs_input.py
+-rw-r--r--   0        0        0    30698 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/subgrid.py
+-rw-r--r--   0        0        0    28381 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/utils.py
+-rw-r--r--   0        0        0      198 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/workflows/__init__.py
+-rw-r--r--   0        0        0    12800 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/workflows/bathymetry.py
+-rw-r--r--   0        0        0     3105 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/workflows/curvenumber.py
+-rw-r--r--   0        0        0     3374 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/workflows/discharge.py
+-rw-r--r--   0        0        0     5285 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/workflows/flwdir.py
+-rw-r--r--   0        0        0      630 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/workflows/landuse.py
+-rw-r--r--   0        0        0    11493 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/workflows/merge.py
+-rw-r--r--   0        0        0    12754 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/hydromt_sfincs/workflows/tiling.py
+-rw-r--r--   0        0        0     1916 2023-08-03 16:01:19.585180 hydromt_sfincs-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6965 1970-01-01 00:00:00.000000 hydromt_sfincs-1.0.1/PKG-INFO
```

### Comparing `hydromt_sfincs-1.0.0/.gitignore` & `hydromt_sfincs-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hydromt_sfincs-1.0.0/LICENSE` & `hydromt_sfincs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydromt_sfincs-1.0.0/README.rst` & `hydromt_sfincs-1.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 HydroMT-SFINCS aims to make the model building process **fast**, **modular** and **reproducible**
 and to facilitate the analysis of SFINCS model results
 
 How to use HydroMT-SFINCS?
 --------------------------
 The HydroMT-SFINCS plugin can be used as a **command line + configuration file** application, which provides commands to *build*,
 *update* the SFINCS model with a single line, or **from python** to exploit its rich interface.
-You can learn more about how to use HydroMT-SFINCS in its `online documentation. <docs_getting_started>`_
+You can learn more about how to use HydroMT-SFINCS in its `online documentation. <https://deltares.github.io/hydromt_sfincs/latest/getting_started/intro>`_
 For a smooth installing experience we recommend installing HydroMT-SFINCS and its dependencies
-from conda-forge in a clean environment, see `installation guide. <docs_install>`_
+from conda-forge in a clean environment, see `installation guide. <https://deltares.github.io/hydromt_sfincs/latest/getting_started/installation>`_
 
 How to cite?
 ------------
 To reference the software please use the the DOI provided in the Zenodo badge that points to the latest release |doi|.
 
 The following paper presents a real-world application of HydroMT-SFINCS:
 
@@ -54,16 +54,14 @@
 You can find information about how to contribute to the HydroMT project at our `contributing page. <https://deltares.github.io/hydromt/latest/dev/contributing>`_
 
 HydroMT seeks active contribution from the (hydro) geoscientific community.
 So far, it has been developed and tested with a range of `Deltares <https://www.deltares.nl/en/>`_ models, but
 we believe it is applicable to a much wider set of geoscientific models and are
 happy to discuss how it can be implemented for your model.
 
-.. _docs_getting_started: https://deltares.github.io/hydromt_sfincs/latest/getting_started/intro
-.. _docs_install: https://deltares.github.io/hydromt_sfincs/latest/getting_started/installation
 .. _Hydromt: https://deltares.github.io/hydromt/latest/
 .. _SFINCS: https://sfincs.readthedocs.io/en/latest/
 
 .. |codecov| image:: https://codecov.io/gh/Deltares/hydromt_sfincs/branch/main/graph/badge.svg?token=ss3EgmwHhH
     :target: https://codecov.io/gh/Deltares/hydromt_sfincs
 
 .. |docs_latest| image:: https://img.shields.io/badge/docs-latest-brightgreen.svg
```

### Comparing `hydromt_sfincs-1.0.0/environment.yml` & `hydromt_sfincs-1.0.1/environment.yml`

 * *Files identical despite different names*

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/corine_mapping.csv` & `hydromt_sfincs-1.0.1/hydromt_sfincs/data/lulc/corine_mapping.csv`

 * *Files identical despite different names*

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/globcover_mapping.csv` & `hydromt_sfincs-1.0.1/hydromt_sfincs/data/lulc/globcover_mapping.csv`

 * *Files identical despite different names*

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/vito_mapping.csv` & `hydromt_sfincs-1.0.1/hydromt_sfincs/data/lulc/vito_mapping.csv`

 * *Files identical despite different names*

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/data/sfincs/sfincs.inp` & `hydromt_sfincs-1.0.1/hydromt_sfincs/data/sfincs/sfincs.inp`

 * *Files identical despite different names*

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/plots.py` & `hydromt_sfincs-1.0.1/hydromt_sfincs/plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 
 from .utils import get_bounds_vector
 
 __all__ = ["plot_forcing", "plot_basemap"]
 
 geom_style = {
     "rivers": dict(linestyle="-", linewidth=1.0, color="darkblue"),
-    "rivers_out": dict(linestyle="-", linewidth=1.0, color="darkgreen"),
+    "rivers_inflow": dict(linestyle=":", linewidth=1.0, color="darkblue"),
+    "rivers_outflow": dict(linestyle=":", linewidth=1.0, color="darkgreen"),
     "msk2": dict(linestyle="-", linewidth=1.5, color="r"),
     "msk3": dict(linestyle="-", linewidth=1.5, color="m"),
     "thd": dict(linestyle="-", linewidth=1.0, color="k", annotate=False),
     "weir": dict(linestyle="--", linewidth=1.0, color="k", annotate=False),
     "bnd": dict(marker="^", markersize=75, c="w", edgecolor="k", annotate=True),
     "src": dict(marker=">", markersize=75, c="w", edgecolor="k", annotate=True),
     "obs": dict(marker="d", markersize=75, c="w", edgecolor="r", annotate=True),
+    "crs": dict(linestyle="-", linewidth=1.5, color="deeppink", annotate=False),
     "region": dict(ls="--", linewidth=1, color="r"),
 }
 
 
 def plot_forcing(forcing: Dict, **kwargs):
     """Plot model timeseries forcing.
 
@@ -48,24 +50,45 @@
     axes = [axes] if n == 1 else axes
     for i, name in enumerate(forcing):
         da = forcing[name].transpose("time", ...)
         longname = da.attrs.get("standard_name", "")
         unit = da.attrs.get("unit", "")
         prefix = ""
         if da.ndim == 3:
-            da = da.mean(dim=[da.raster.x_dim, da.raster.y_dim])
-            prefix = "mean "
+            if name.startswith("press"):
+                da = da.min(dim=[da.raster.x_dim, da.raster.y_dim])
+                prefix = "min "
+            elif name.startswith("wind_u") or name.startswith("wind_v"):
+                da = da.max(dim=[da.raster.x_dim, da.raster.y_dim])
+                prefix = "max "
+            else:
+                da = da.mean(dim=[da.raster.x_dim, da.raster.y_dim])
+                prefix = "mean "
         # convert to Single index dataframe (bar plots don't work with xarray)
         df = da.to_pandas()
         if isinstance(df.index, pd.MultiIndex):
             df = df.unstack(0)
         # convert dates a-priori as automatic conversion doesn't always work
         df.index = mdates.date2num(df.index)
         if name.startswith("precip"):
             axes[i].bar(df.index, df.values, facecolor="darkblue")
+        elif (
+            name.startswith("press")
+            or name.startswith("wind_u")
+            or name.startswith("wind_v")
+        ):
+            df.plot.line(ax=axes[i])
+        elif name.startswith("wnd"):
+            df.plot(ax=axes[i], kind="line", secondary_y="dir", legend=False)
+            # set tick color for y-axis of variable 1
+            axes[i].tick_params(axis="y", labelcolor="C0")
+            axes[i].right_ax.set_ylabel("Wind direction [degrees]")
+            # set tick color and label for y-axis of variable 2
+            axes[i].right_ax.tick_params(axis="y", labelcolor="C1")
+
         else:
             df.plot.line(ax=axes[i]).legend(
                 title="index",
                 bbox_to_anchor=(1.05, 1),
                 loc="upper left",
                 ncol=df.columns.size // 5 + 1,
                 prop={"size": 8},
@@ -138,28 +161,36 @@
     """
     import cartopy.crs as ccrs
     import cartopy.io.img_tiles as cimgt
     import matplotlib.pyplot as plt
     from matplotlib import colors, patheffects
 
     # read crs and utm zone > convert to cartopy
-    wkt = ds.raster.crs.to_wkt()
-    if "UTM zone " not in wkt:
-        raise ValueError("Model CRS UTM zone not found.")
-    utm_zone = ds.raster.crs.to_wkt().split("UTM zone ")[1][:3]
-    utm = ccrs.UTM(int(utm_zone[:2]), "S" in utm_zone)
-    extent = np.array(ds.raster.box.buffer(1e2).total_bounds)[[0, 2, 1, 3]]
+    proj_crs = ds.raster.crs
+    proj_str = proj_crs.name
+    if proj_crs.is_projected and proj_crs.to_epsg() is not None:
+        crs = ccrs.epsg(ds.raster.crs.to_epsg())
+        unit = proj_crs.axis_info[0].unit_name
+        unit = "m" if unit == "metre" else unit
+        xlab, ylab = f"x [{unit}] - {proj_str}", f"y [{unit}]"
+    elif proj_crs.is_geographic:
+        crs = ccrs.PlateCarree()
+        xlab, ylab = f"lon [deg] - {proj_str}", "lat [deg]"
+    else:
+        raise ValueError("Unsupported CRS")
+    bounds = ds.raster.box.buffer(abs(ds.raster.res[0] * 1)).total_bounds
+    extent = np.array(bounds)[[0, 2, 1, 3]]
 
     # create fig with geo-axis and set background
     if figsize is None:
         ratio = ds.raster.ycoords.size / (ds.raster.xcoords.size * 1.4)
         figsize = (8, 8 * ratio)
     fig = plt.figure(figsize=figsize)
-    ax = plt.subplot(projection=utm)
-    ax.set_extent(extent, crs=utm)
+    ax = plt.subplot(projection=crs)
+    ax.set_extent(extent, crs=crs)
     if bmap == "sat":
         ax.add_image(cimgt.QuadtreeTiles(**bmap_kwargs), zoomlevel)
     elif bmap == "osm":
         ax.add_image(cimgt.OSM(**bmap_kwargs), zoomlevel)
     elif bmap is not None and hasattr(cimgt, bmap):
         ax.add_image(getattr(cimgt, bmap)(**bmap_kwargs), zoomlevel)
 
@@ -177,28 +208,28 @@
                 c_dem = np.vstack((c_bat, c_dem))
             cmap = colors.LinearSegmentedColormap.from_list("dem", c_dem)
             norm = colors.Normalize(vmin=vmin, vmax=vmax)
             cmap, norm = kwargs.pop("cmap", cmap), kwargs.pop("norm", norm)
             kwargs0.update(norm=norm, cmap=cmap)
         elif variable == "msk" and "msk" in ds:
             cmap = colors.LinearSegmentedColormap.from_list(
-                "Set1", ["grey", "r", "m"], N=4
+                "Set1", ["grey", "r", "m"], N=3
             )
             norm = colors.BoundaryNorm([0.5, 1.5, 2.5, 3.5], 3)
             kwargs0.update(norm=norm, cmap=cmap)
             kwargs0["cbar_kwargs"].update(ticks=[1, 2, 3])
 
     if variable in ds:
         da = ds[variable].raster.mask_nodata()
         if np.any(ds["msk"] > 0):
             da = da.where(ds["msk"] > 0)
         if da.raster.rotation != 0 and "xc" in da.coords and "yc" in da.coords:
-            da.plot(transform=utm, x="xc", y="yc", ax=ax, zorder=1, **kwargs0)
+            da.plot(transform=crs, x="xc", y="yc", ax=ax, zorder=1, **kwargs0)
         else:
-            da.plot.imshow(transform=utm, ax=ax, zorder=1, **kwargs0)
+            da.plot.imshow(transform=crs, ax=ax, zorder=1, **kwargs0)
         if shaded and variable == "dep" and da.raster.rotation == 0:
             ls = colors.LightSource(azdeg=315, altdeg=45)
             dx, dy = da.raster.res
             _rgb = ls.shade(
                 da.fillna(0).values,
                 norm=kwargs["norm"],
                 cmap=kwargs["cmap"],
@@ -207,15 +238,15 @@
                 dy=dy,
                 vert_exag=2,
             )
             rgb = xr.DataArray(
                 dims=("y", "x", "rgb"), data=_rgb, coords=da.raster.coords
             )
             rgb = xr.where(np.isnan(da), np.nan, rgb)
-            rgb.plot.imshow(transform=utm, ax=ax, zorder=1)
+            rgb.plot.imshow(transform=crs, ax=ax, zorder=1)
 
     # geometry plotting and annotate kwargs
     for k, d in geom_kwargs.items():
         geom_style[k].update(**d)
     ann_kwargs = dict(
         xytext=(3, 3),
         textcoords="offset points",
@@ -255,16 +286,16 @@
         geoms["region"].boundary.plot(
             ax=ax, zorder=2, label="region", **geom_style["region"]
         )
 
     # title, legend and labels
     ax.xaxis.set_visible(True)
     ax.yaxis.set_visible(True)
-    ax.set_ylabel(f"y coordinate UTM zone {utm_zone} [m]")
-    ax.set_xlabel(f"x coordinate UTM zone {utm_zone} [m]")
+    ax.set_ylabel(ylab)
+    ax.set_xlabel(xlab)
     variable = "base" if variable is None else variable
     ax.set_title(f"SFINCS {variable} map")
     # NOTE without defined loc it takes forever to find a 'best' location
     # by default outside plot
     if geom_names or plot_bounds:
         legend_kwargs0 = dict(
             bbox_to_anchor=(1.05, 1),
```

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/regulargrid.py` & `hydromt_sfincs-1.0.1/hydromt_sfincs/regulargrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         gdf_exclude: gpd.GeoDataFrame = None,
         zmin: float = None,
         zmax: float = None,
         fill_area: float = 10,
         drop_area: float = 0,
         connectivity: int = 8,
         all_touched: bool = True,
-        reset_mask: bool = False,
+        reset_mask: bool = True,
         logger: logging.Logger = logger,
     ) -> xr.DataArray:
         """Create an integer mask with inactive (msk=0) and active (msk=1) cells, optionally bounded
         by several criteria.
 
         Parameters
         ----------
@@ -175,15 +175,15 @@
             The connectivity used to define contiguous cells, if 4 only horizontal and vertical
             connections are used, if 8 (default) also diagonal connections.
         all_touched: bool, optional
             if True (default) include (or exclude) a cell in the mask if it touches any of the
             include (or exclude) geometries. If False, include a cell only if its center is
             within one of the shapes, or if it is selected by Bresenham's line algorithm.
         reset_mask: bool, optional
-            If True, reset existing mask layer. If False (default) updating existing mask.
+            If True (default), reset existing mask layer. If False updating existing mask.
 
         Returns
         -------
         da_mask: xr.DataArray
             Integer SFINCS model mask with inactive (msk=0), active (msk=1) cells
         """
```

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/sfincs.py` & `hydromt_sfincs-1.0.1/hydromt_sfincs/sfincs.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 import hydromt
 import numpy as np
 import pandas as pd
 import xarray as xr
 from hydromt.models.model_grid import GridModel
 from hydromt.raster import RasterDataArray
 from hydromt.vector import GeoDataArray, GeoDataset
+from hydromt.workflows.forcing import da_to_timedelta
 from pyproj import CRS
-from shapely.geometry import box
+from shapely.geometry import box, LineString, MultiLineString, Polygon
 
 from . import DATADIR, plots, utils, workflows
 from .regulargrid import RegularGrid
 from .sfincs_input import SfincsInput
 
 __all__ = ["SfincsModel"]
 
@@ -33,36 +34,42 @@
 class SfincsModel(GridModel):
     # GLOBAL Static class variables that can be used by all methods within
     # SfincsModel class. Typically list of variables (e.g. _MAPS) or
     # dict with varname - filename pairs (e.g. thin_dams : thd)
     _NAME = "sfincs"
     _GEOMS = {
         "observation_points": "obs",
+        "observation_lines": "crs",
         "weirs": "weir",
         "thin_dams": "thd",
+        "drainage_structures": "drn",
     }  # parsed to dict of geopandas.GeoDataFrame
     _FORCING_1D = {
         # timeseries (can be multiple), locations tuple
         "waterlevel": (["bzs"], "bnd"),
         "waves": (["bzi"], "bnd"),
         "discharge": (["dis"], "src"),
         "precip": (["precip"], None),
+        "wind": (["wnd"], None),
         "wavespectra": (["bhs", "btp", "bwd", "bds"], "bwv"),
         "wavemaker": (["whi", "wti", "wst"], "wvp"),  # TODO check names and test
     }
     _FORCING_NET = {
         # 2D forcing sfincs name, rename tuple
         "waterlevel": ("netbndbzsbzi", {"zs": "bzs", "zi": "bzi"}),
         "discharge": ("netsrcdis", {"discharge": "dis"}),
-        "precip": ("netampr", {"Precipitation": "precip"}),
-        "press": ("netamp", {"barometric_pressure": "press"}),
-        "wind": ("netamuamv", {"eastward_wind": "wind_u", "northward_wind": "wind_v"}),
+        "precip_2d": ("netampr", {"Precipitation": "precip_2d"}),
+        "press_2d": ("netamp", {"barometric_pressure": "press_2d"}),
+        "wind_2d": (
+            "netamuamv",
+            {"eastward_wind": "wind_u", "northward_wind": "wind_v"},
+        ),
     }
     _FORCING_SPW = {"spiderweb": "spw"}  # TODO add read and write functions
-    _MAPS = ["msk", "dep", "scs", "manning", "qinf"]
+    _MAPS = ["msk", "dep", "scs", "manning", "qinf", "smax", "seff", "kr"]
     _STATES = ["rst", "ini"]
     _FOLDERS = []
     _CLI_ARGS = {"region": "setup_grid_from_region", "res": "setup_grid_from_region"}
     _CONF = "sfincs.inp"
     _DATADIR = DATADIR
     _ATTRS = {
         "dep": {"standard_name": "elevation", "unit": "m+ref"},
@@ -73,14 +80,19 @@
         },
         "qinf": {"standard_name": "infiltration rate", "unit": "mm.hr-1"},
         "manning": {"standard_name": "manning roughness", "unit": "s.m-1/3"},
         "bzs": {"standard_name": "waterlevel", "unit": "m+ref"},
         "bzi": {"standard_name": "wave height", "unit": "m"},
         "dis": {"standard_name": "discharge", "unit": "m3.s-1"},
         "precip": {"standard_name": "precipitation", "unit": "mm.hr-1"},
+        "precip_2d": {"standard_name": "precipitation", "unit": "mm.hr-1"},
+        "press_2d": {"standard_name": "barometric pressure", "unit": "Pa"},
+        "wind_u": {"standard_name": "eastward wind", "unit": "m/s"},
+        "wind_v": {"standard_name": "northward wind", "unit": "m/s"},
+        "wnd": {"standard_name": "wind", "unit": "m/s"},
     }
 
     def __init__(
         self,
         root: str = None,
         mode: str = "w",
         config_fn: str = "sfincs.inp",
@@ -329,22 +341,23 @@
                 da_like=self.mask,
                 buffer_cells=buffer_cells,
                 interp_method=interp_method,
                 logger=self.logger,
             )
 
             # check if no nan data is present in the bed levels
-            if not np.isnan(da_dep).any():
+            if np.isnan(da_dep).any():
                 self.logger.warning(
                     f"Interpolate data at {int(np.sum(np.isnan(da_dep.values)))} cells"
                 )
+                # TODO add extrapolate=True option when available in hydromt core
                 da_dep = da_dep.raster.interpolate_na(method="rio_idw")
 
             self.set_grid(da_dep, name="dep")
-            # FIXME this shouldn't be necessary, since da_dep should already have the crs
+            # FIXME this shouldn't be necessary, since da_dep should already have a crs
             if self.crs is not None and self.grid.raster.crs is None:
                 self.grid.set_crs(self.crs)
 
             if "depfile" not in self.config:
                 self.config.update({"depfile": "sfincs.dep"})
         elif self.grid_type == "quadtree":
             raise NotImplementedError(
@@ -359,15 +372,15 @@
         mask_buffer: int = 0,
         zmin: float = None,
         zmax: float = None,
         fill_area: float = 10.0,
         drop_area: float = 0.0,
         connectivity: int = 8,
         all_touched: bool = True,
-        reset_mask: bool = False,
+        reset_mask: bool = True,
     ):
         """Setup active model cells.
 
         The SFINCS model mask defines inactive (msk=0), active (msk=1), and waterlevel boundary (msk=2)
         and outflow boundary (msk=3) cells. This method sets the active and inactive cells.
 
         Active model cells are based on a region and cells with valid elevation (i.e. not nodata),
@@ -403,15 +416,15 @@
             The connectivity used to define contiguous cells, if 4 only horizontal and vertical
             connections are used, if 8 (default) also diagonal connections.
         all_touched: bool, optional
             if True (default) include (or exclude) a cell in the mask if it touches any of the
             include (or exclude) geometries. If False, include a cell only if its center is
             within one of the shapes, or if it is selected by Bresenham's line algorithm.
         reset_mask: bool, optional
-            If True, reset existing mask layer. If False (default) updating existing mask.
+            If True  (default), reset existing mask layer. If False updating existing mask.
         """
         # read geometries
         gdf_mask, gdf_include, gdf_exclude = None, None, None
         bbox = self.region.to_crs(4326).total_bounds
         if mask is not None:
             if not isinstance(mask, gpd.GeoDataFrame) and str(mask).endswith(".pol"):
                 # NOTE polygons should be in same CRS as model
@@ -466,17 +479,23 @@
             self.set_grid(da_mask, name="msk")
             # update config
             if "mskfile" not in self.config:
                 self.config.update({"mskfile": "sfincs.msk"})
             if "indexfile" not in self.config:
                 self.config.update({"indexfile": "sfincs.ind"})
             # update region
-            self.logger.info("Derive region geometry based on active cells.")
-            region = da_mask.where(da_mask <= 1, 1).raster.vectorize()
-            self.set_geoms(region, "region")
+            if np.any(da_mask >= 1):
+                self.logger.info("Derive region geometry based on active cells.")
+                # make mask with ones and zeros only -> vectorize ones
+                region = da_mask.where(da_mask <= 1, 1).raster.vectorize()
+                if region.empty:
+                    raise ValueError("No region found.")
+                self.set_geoms(region, "region")
+            else:
+                self.logger.warning("No active cells found.")
 
     def setup_mask_bounds(
         self,
         btype: str = "waterlevel",
         include_mask: Union[str, Path, gpd.GeoDataFrame] = None,
         exclude_mask: Union[str, Path, gpd.GeoDataFrame] = None,
         zmin: float = None,
@@ -502,34 +521,35 @@
         * **msk** map: model mask [-]
 
         Parameters
         ----------
         btype: {'waterlevel', 'outflow'}
             Boundary type
         include_mask, exclude_mask: str, Path, gpd.GeoDataFrame, optional
-            Path or data source name for geometries with areas to include/exclude from the model boundary.
+            Path or data source name for geometries with areas to include/exclude from
+            the model boundary.
         zmin, zmax : float, optional
             Minimum and maximum elevation thresholds for boundary cells.
-            Note that when include and exclude areas are used, the elevation range is only applied
-            on cells within the include area and outside the exclude area.
+            Note that when include and exclude areas are used, the elevation range is
+            only applied on cells within the include area and outside the exclude area.
         reset_bounds: bool, optional
             If True, reset existing boundary cells of the selected boundary
             type (`btype`) before setting new boundary cells, by default False.
         all_touched: bool, optional
             if True (default) include (or exclude) a cell in the mask if it touches any of the
             include (or exclude) geometries. If False, include a cell only if its center is
             within one of the shapes, or if it is selected by Bresenham's line algorithm.
         connectivity, {4, 8}:
             The connectivity used to detect the model edge, if 4 only horizontal and vertical
             connections are used, if 8 (default) also diagonal connections.
         """
 
         # get include / exclude geometries
         gdf_include, gdf_exclude = None, None
-        bbox = self.region.to_crs(4326).total_bounds
+        bbox = self.mask.raster.transform_bounds(4326)
         if include_mask is not None:
             if not isinstance(include_mask, gpd.GeoDataFrame) and str(
                 include_mask
             ).endswith(".pol"):
                 # NOTE polygons should be in same CRS as model
                 gdf_include = utils.polygon2gdf(
                     feats=utils.read_geoms(fn=include_mask), crs=self.region.crs
@@ -567,23 +587,25 @@
             )
             self.set_grid(da_mask, name="msk")
 
     def setup_subgrid(
         self,
         datasets_dep: List[dict],
         datasets_rgh: List[dict] = [],
+        datasets_riv: List[dict] = [],
         buffer_cells: int = 0,
         nbins: int = 10,
         nr_subgrid_pixels: int = 20,
         nrmax: int = 2000,  # blocksize
         max_gradient: float = 5.0,
         z_minimum: float = -99999.0,
         manning_land: float = 0.04,
         manning_sea: float = 0.02,
         rgh_lev_land: float = 0.0,
+        extrapolate_values: bool = False,
         write_dep_tif: bool = False,
         write_man_tif: bool = False,
     ):
         """Setup method for subgrid tables based on a list of
         elevation and Manning's roughness datasets.
 
         These datasets are used to derive relations between the water level
@@ -593,45 +615,75 @@
         This allows that one can compute on a coarser computational grid,
         while still accounting for the local topography and roughness.
 
         Parameters
         ----------
         datasets_dep : List[dict]
             List of dictionaries with topobathy data.
-            Each should minimally contain a data catalog source name, data file path, or xarray raster object ('elevtn')
-            Optional merge arguments include 'zmin', 'zmax', 'mask', 'offset', 'reproj_method', and 'merge_method'.
-            e.g.: [{'elevtn': merit_hydro, 'zmin': 0.01}, {'elevtn': gebco, 'offset': 0, 'merge_method': 'first', reproj_method: 'bilinear'}]
-            For a complete overview of all merge options, see :py:function:~hydromt.workflows.merge_multi_dataarrays
+            Each should minimally contain a data catalog source name, data file path,
+            or xarray raster object ('elevtn'). Optional merge arguments include:
+            'zmin', 'zmax', 'mask', 'offset', 'reproj_method', and 'merge_method'.
+            e.g.: [
+                {'elevtn': 'merit_hydro', 'zmin': 0.01},
+                {'elevtn': 'gebco', 'offset': 0, 'merge_method': 'first', reproj_method: 'bilinear'}
+            ]
+            For a complete overview of all merge options, see
+            :py:function:~hydromt.workflows.merge_multi_dataarrays
         datasets_rgh : List[dict], optional
-            List of dictionaries with Manning's n datasets. Each dictionary should at least contain one of the following:
+            List of dictionaries with Manning's n datasets. Each dictionary should at
+            least contain one of the following:
             * (1) manning: filename (or Path) of gridded data with manning values
-            * (2) lulc (and reclass_table) :a combination of a filename of gridded landuse/landcover and a mapping table.
-            In additon, optional merge arguments can be provided e.g.: merge_method, gdf_valid_fn
+            * (2) lulc (and reclass_table) :a combination of a filename of gridded
+            landuse/landcover and a mapping table. In additon, optional merge arguments
+            can be provided, e.g.: [
+                {'manning': 'manning_data'},
+                {'lulc': 'esa_worlcover', 'reclass_table': 'esa_worlcover_mapping'}
+            ]
+        datasets_riv : List[dict], optional
+            List of dictionaries with river datasets. Each dictionary should at least
+            contain a river centerline data and optionally a river mask:
+            * centerlines: filename (or Path) of river centerline with attributes
+                rivwth (river width [m]; required if not river mask provided),
+                rivdph or rivbed (river depth [m]; river bedlevel [m+REF]),
+                manning (Manning's n [s/m^(1/3)]; optional)
+            * mask (optional): filename (or Path) of river mask
+            * river attributes (optional): "rivdph", "rivbed", "rivwth", "manning"
+                to fill missing values
+            * arguments to the river burn method (optional):
+                segment_length [m] (default 500m) and riv_bank_q [0-1] (default 0.5)
+                which used to estimate the river bank height in case river depth is provided.
+              For more info see :py:function:~hydromt.workflows.bathymetry.burn_river_rect
+           e.g.: [{'centerlines': 'river_lines', 'mask': 'river_mask', 'manning': 0.035}]
         buffer_cells : int, optional
-            Number of cells between datasets to ensure smooth transition of bed levels, by default 0
+            Number of cells between datasets to ensure smooth transition of bed levels,
+            by default 0
         nbins : int, optional
-            Number of bins in the subgrid tables, by default 10
+            Number of bins in which hypsometry is subdivided, by default 10
         nr_subgrid_pixels : int, optional
             Number of subgrid pixels per computational cell, by default 20
         nrmax : int, optional
             Maximum number of cells per subgrid-block, by default 2000
             These blocks are used to prevent memory issues while working with large datasets
         max_gradient : float, optional
-            Maximum gradient in the subgrid tables, by default 5.0
+            If slope in hypsometry exceeds this value, then smoothing is applied,
+            to prevent numerical stability problems, by default 5.0
         z_minimum : float, optional
             Minimum depth in the subgrid tables, by default -99999.0
         manning_land, manning_sea : float, optional
             Constant manning roughness values for land and sea, by default 0.04 and 0.02 s.m-1/3
-            Note that these values are only used when no Manning's n datasets are provided, or to fill the nodata values
+            Note that these values are only used when no Manning's n datasets are provided,
+            or to fill the nodata values
         rgh_lev_land : float, optional
-            Elevation level to distinguish land and sea roughness (when using manning_land and manning_sea), by default 0.0
-        write_dep_tif : bool, optional
-            Create geotiff of the merged topobathy on the subgrid resolution, by default False
-        write_man_tif : bool, optional
-            Create geotiff of the merged roughness on the subgrid resolution, by default False
+            Elevation level to distinguish land and sea roughness
+            (when using manning_land and manning_sea), by default 0.0
+        write_dep_tif, write_man_tif : bool, optional
+            Write geotiff of the merged topobathy / roughness on the subgrid resolution.
+            These files are not used by SFINCS, but can be used for visualisation and
+            downscaling of the floodmaps. Unlinke the SFINCS files it is written
+            to disk at execution of this method. By default False
         """
 
         # retrieve model resolution
         # TODO fix for quadtree
         if not self.mask.raster.crs.is_geographic:
             res = np.abs(self.mask.raster.res[0]) / nr_subgrid_pixels
         else:
@@ -639,38 +691,43 @@
 
         datasets_dep = self._parse_datasets_dep(datasets_dep, res=res)
 
         if len(datasets_rgh) > 0:
             # NOTE conversion from landuse/landcover to manning happens here
             datasets_rgh = self._parse_datasets_rgh(datasets_rgh)
 
+        if len(datasets_riv) > 0:
+            datasets_riv = self._parse_datasets_riv(datasets_riv)
+
         # folder where high-resolution topobathy and manning geotiffs are stored
         if write_dep_tif or write_man_tif:
             highres_dir = os.path.join(self.root, "subgrid")
             if not os.path.isdir(highres_dir):
                 os.makedirs(highres_dir)
         else:
             highres_dir = None
 
         if self.grid_type == "regular":
             self.reggrid.subgrid.build(
                 da_mask=self.mask,
                 datasets_dep=datasets_dep,
                 datasets_rgh=datasets_rgh,
+                datasets_riv=datasets_riv,
                 buffer_cells=buffer_cells,
                 nbins=nbins,
                 nr_subgrid_pixels=nr_subgrid_pixels,
                 nrmax=nrmax,
                 max_gradient=max_gradient,
                 z_minimum=z_minimum,
                 manning_land=manning_land,
                 manning_sea=manning_sea,
                 rgh_lev_land=rgh_lev_land,
                 write_dep_tif=write_dep_tif,
                 write_man_tif=write_man_tif,
+                extrapolate_values=extrapolate_values,
                 highres_dir=highres_dir,
                 logger=self.logger,
             )
             self.subgrid = self.reggrid.subgrid.to_xarray(
                 dims=self.mask.raster.dims, coords=self.mask.raster.coords
             )
         elif self.grid_type == "quadtree":
@@ -745,15 +802,15 @@
         setup_discharge_forcing
         setup_discharge_forcing_from_grid
         """
         da_flwdir, da_uparea, gdf_riv = None, None, None
         if hydrography is not None:
             ds = self.data_catalog.get_rasterdataset(
                 hydrography,
-                geom=self.region,
+                bbox=self.mask.raster.transform_bounds(4326),
                 variables=["uparea", "flwdir"],
                 buffer=5,
             )
             da_flwdir = ds["flwdir"]
             da_uparea = ds["uparea"]
         elif rivers == "rivers_outflow" and rivers in self.geoms:
             # reuse rivers from setup_river_in/outflow
@@ -864,15 +921,15 @@
         --------
         setup_mask_bounds
         """
         da_flwdir, da_uparea, gdf_riv = None, None, None
         if hydrography is not None:
             ds = self.data_catalog.get_rasterdataset(
                 hydrography,
-                geom=self.region,
+                bbox=self.mask.raster.transform_bounds(4326),
                 variables=["uparea", "flwdir"],
                 buffer=5,
             )
             da_flwdir = ds["flwdir"]
             da_uparea = ds["uparea"]
         elif rivers == "rivers_inflow" and rivers in self.geoms:
             # reuse rivers from setup_river_in/outflow
@@ -921,35 +978,74 @@
         elif reset_bounds:
             self.setup_mask_bounds(btype=btype, reset_bounds=reset_bounds)
 
         # keep river centerlines
         if keep_rivers_geom and len(gdf_riv) > 0:
             self.set_geoms(gdf_riv, name="rivers_outflow")
 
-    def setup_constant_infiltration(self, qinf, reproj_method="average"):
+    # Function to create constant spatially varying infiltration
+    def setup_constant_infiltration(
+        self,
+        qinf=None,
+        lulc=None,
+        reclass_table=None,
+        reproj_method="average",
+    ):
         """Setup spatially varying constant infiltration rate (qinffile).
 
         Adds model layers:
 
         * **qinf** map: constant infiltration rate [mm/hr]
 
         Parameters
         ----------
         qinf : str, Path, or RasterDataset
             Spatially varying infiltration rates [mm/hr]
+        lulc: str, Path, or RasterDataset
+            Landuse/landcover data set
+        reclass_table: str, Path, or pd.DataFrame
+            Reclassification table to convert landuse/landcover to infiltration rates [mm/hr]
         reproj_method : str, optional
             Resampling method for reprojecting the infiltration data to the model grid.
             By default 'average'. For more information see, :py:meth:`hydromt.raster.RasterDataArray.reproject_like`
         """
 
         # get infiltration data
-        da_inf = self.data_catalog.get_rasterdataset(qinf, geom=self.region, buffer=10)
-        da_inf = da_inf.raster.mask_nodata()  # set nodata to nan
+        if qinf is not None:
+            da_inf = self.data_catalog.get_rasterdataset(
+                qinf,
+                bbox=self.mask.raster.transform_bounds(4326),
+                buffer=10,
+            )
+        elif lulc is not None:
+            # landuse/landcover should always be combined with mapping
+            if reclass_table is None:
+                raise IOError(
+                    f"Infiltration mapping file should be provided for {lulc}"
+                )
+            da_lulc = self.data_catalog.get_rasterdataset(
+                lulc,
+                bbox=self.mask.raster.transform_bounds(4326),
+                buffer=10,
+                variables=["lulc"],
+            )
+            df_map = self.data_catalog.get_dataframe(
+                reclass_table,
+                variables=["qinf"],
+                index_col=0,  # driver kwargs
+            )
+            # reclassify
+            da_inf = da_lulc.raster.reclassify(df_map)["qinf"]
+        else:
+            raise ValueError(
+                "Either qinf or lulc must be provided when setting up constant infiltration."
+            )
 
         # reproject infiltration data to model grid
+        da_inf = da_inf.raster.mask_nodata()  # set nodata to nan
         da_inf = da_inf.raster.reproject_like(self.mask, method=reproj_method)
 
         # check on nan values
         if np.logical_and(np.isnan(da_inf), self.mask >= 1).any():
             self.logger.warning("NaN values found in infiltration data; filled with 0")
             da_inf = da_inf.fillna(0)
         da_inf.raster.set_nodata(-9999.0)
@@ -959,14 +1055,15 @@
         da_inf.attrs.update(**self._ATTRS.get(mname, {}))
         self.set_grid(da_inf, name=mname)
 
         # update config: remove default inf and set qinf map
         self.set_config(f"{mname}file", f"sfincs.{mname}")
         self.config.pop("qinf", None)
 
+    # Function to create curve number for SFINCS
     def setup_cn_infiltration(self, cn, antecedent_moisture="avg", reproj_method="med"):
         """Setup model potential maximum soil moisture retention map (scsfile)
         from gridded curve number map.
 
         Adds model layers:
 
         * **scs** map: potential maximum soil moisture retention [inch]
@@ -983,15 +1080,17 @@
             None if data has no antecedent runoff conditions.
             By default `avg`
         reproj_method : str, optional
             Resampling method for reprojecting the curve number data to the model grid.
             By default 'med'. For more information see, :py:meth:`hydromt.raster.RasterDataArray.reproject_like`
         """
         # get data
-        da_org = self.data_catalog.get_rasterdataset(cn, geom=self.region, buffer=10)
+        da_org = self.data_catalog.get_rasterdataset(
+            cn, bbox=self.mask.raster.transform_bounds(4326), buffer=10
+        )
         # read variable
         v = "cn"
         if antecedent_moisture:
             v = f"cn_{antecedent_moisture}"
         if isinstance(da_org, xr.Dataset) and v in da_org.data_vars:
             da_org = da_org[v]
         elif not isinstance(da_org, xr.DataArray):
@@ -1007,14 +1106,144 @@
         mname = "scs"
         da_scs.attrs.update(**self._ATTRS.get(mname, {}))
         self.set_grid(da_scs, name=mname)
         # update config: remove default infiltration values and set scs map
         self.config.pop("qinf", None)
         self.set_config(f"{mname}file", f"sfincs.{mname}")
 
+    # Function to create curve number for SFINCS including recovery term (Kr)
+    def setup_cn_infiltration_with_kr(
+        self, lulc, hsg, ksat, reclass_table, effective, block_size=2000
+    ):
+        """Setup model the Soil Conservation Service (SCS) Curve Number (CN) files for SFINCS
+        including recovery term based on the soil saturation
+
+        Parameters
+        ---------
+        lulc : str, Path, or RasterDataset
+            Landuse/landcover data set
+        hsg : str, Path, or RasterDataset
+            HSG (Hydrological Similarity Group) in integers
+        ksat : str, Path, or RasterDataset
+            Ksat (saturated hydraulic conductivity) [µm/s]
+        reclass_table : str, Path, or RasterDataset
+            reclass table to relate landcover with soiltype
+        effective : float
+            estimate of percentage effective soil, e.g. 0.50 for 50%
+        block_size : float
+            maximum block size - use larger values will get more data in memory but can be faster, default=2000
+        """
+
+        # Read the datafiles
+        da_landuse = self.data_catalog.get_rasterdataset(
+            lulc, bbox=self.mask.raster.transform_bounds(4326), buffer=10
+        )
+        da_HSG = self.data_catalog.get_rasterdataset(
+            hsg, bbox=self.mask.raster.transform_bounds(4326), buffer=10
+        )
+        da_Ksat = self.data_catalog.get_rasterdataset(
+            ksat, bbox=self.mask.raster.transform_bounds(4326), buffer=10
+        )
+        df_map = self.data_catalog.get_dataframe(reclass_table, index_col=0)
+
+        # Define outputs
+        da_smax = xr.full_like(self.mask, -9999, dtype=np.float32)
+        da_kr = xr.full_like(self.mask, -9999, dtype=np.float32)
+
+        # Compute resolution land use (we are assuming that is the finest)
+        resolution_landuse = np.mean(
+            [abs(da_landuse.raster.res[0]), abs(da_landuse.raster.res[1])]
+        )
+        if da_landuse.raster.crs.is_geographic:
+            resolution_landuse = (
+                resolution_landuse * 111111.0
+            )  # assume 1 degree is 111km
+
+        # Define the blocks
+        nrmax = block_size
+        nmax = np.shape(self.mask)[0]
+        mmax = np.shape(self.mask)[1]
+        refi = self.config["dx"] / resolution_landuse  # finest resolution of landuse
+        nrcb = int(np.floor(nrmax / refi))  # nr of regular cells in a block
+        nrbn = int(np.ceil(nmax / nrcb))  # nr of blocks in n direction
+        nrbm = int(np.ceil(mmax / nrcb))  # nr of blocks in m direction
+        x_dim, y_dim = self.mask.raster.x_dim, self.mask.raster.y_dim
+
+        # avoid blocks with width or height of 1
+        merge_last_col = False
+        merge_last_row = False
+        if mmax % nrcb == 1:
+            nrbm -= 1
+            merge_last_col = True
+        if nmax % nrcb == 1:
+            nrbn -= 1
+            merge_last_row = True
+
+        ## Loop through blocks
+        ib = -1
+        for ii in range(nrbm):
+            bm0 = ii * nrcb  # Index of first m in block
+            bm1 = min(bm0 + nrcb, mmax)  # last m in block
+            if merge_last_col and ii == (nrbm - 1):
+                bm1 += 1
+
+            for jj in range(nrbn):
+                bn0 = jj * nrcb  # Index of first n in block
+                bn1 = min(bn0 + nrcb, nmax)  # last n in block
+                if merge_last_row and jj == (nrbn - 1):
+                    bn1 += 1
+
+                # Count
+                ib += 1
+                self.logger.debug(
+                    f"\nblock {ib + 1}/{nrbn * nrbm} -- "
+                    f"col {bm0}:{bm1-1} | row {bn0}:{bn1-1}"
+                )
+
+                # calculate transform and shape of block at cell and subgrid level
+                da_mask_block = self.mask.isel(
+                    {x_dim: slice(bm0, bm1), y_dim: slice(bn0, bn1)}
+                ).load()
+
+                # Call workflow
+                (
+                    da_smax_block,
+                    da_kr_block,
+                ) = workflows.curvenumber.scs_recovery_determination(
+                    da_landuse, da_HSG, da_Ksat, df_map, da_mask_block
+                )
+
+                # New place in the overall matrix
+                sn, sm = slice(bn0, bn1), slice(bm0, bm1)
+                da_smax[sn, sm] = da_smax_block
+                da_kr[sn, sm] = da_kr_block
+
+        # Done
+        self.logger.info(f"Done with determination of values (in blocks).")
+
+        # Specify the effective soil retention (seff)
+        da_seff = da_smax
+        da_seff = da_seff * effective
+        da_seff.raster.set_nodata(da_smax.raster.nodata)
+
+        # set grids for seff, smax and kr
+        names = ["smax", "seff", "kr"]
+        data = [da_smax, da_seff, da_kr]
+        for name, da in zip(names, data):
+            # Give metadata to the layer and set grid
+            da.attrs.update(**self._ATTRS.get(name, {}))
+            self.set_grid(da, name=name)
+
+            # update config: set maps
+            self.set_config(f"{name}file", f"sfincs.{name}")  # give it to SFINCS
+
+        # Remove qinf variable in sfincs
+        self.config.pop("qinf", None)
+
+    # Roughness
     def setup_manning_roughness(
         self,
         datasets_rgh: List[dict] = [],
         manning_land=0.04,
         manning_sea=0.02,
         rgh_lev_land=0,
     ):
@@ -1113,18 +1342,63 @@
             gdf0 = self._geoms.pop(name)
             gdf_obs = gpd.GeoDataFrame(pd.concat([gdf_obs, gdf0], ignore_index=True))
             self.logger.info(f"Adding new observation points to existing ones.")
 
         self.set_geoms(gdf_obs, name)
         self.set_config(f"{name}file", f"sfincs.{name}")
 
+    def setup_observation_lines(
+        self,
+        locations: Union[str, Path, gpd.GeoDataFrame],
+        merge: bool = True,
+        **kwargs,
+    ):
+        """Setup model observation lines (cross-sections) to monitor discharges.
+
+        Adds model layers:
+
+        * **crs** geom: observation lines (cross-sections)
+
+        Parameters
+        ---------
+        locations: str, Path, gpd.GeoDataFrame, optional
+            Path, data source name, or geopandas object for observation lines (cross-sections).
+        merge: bool, optional
+            If True, merge the new observation lines with the existing ones. By default True.
+        """
+        name = self._GEOMS["observation_lines"]
+
+        # FIXME ensure the catalog is loaded before adding any new entries
+        self.data_catalog.sources
+
+        # FIXME assert_gtype="LineString" does not work for MultiLineString and default seems to be Point (??)
+        gdf_obs = self.data_catalog.get_geodataframe(
+            locations, geom=self.region, assert_gtype=None, **kwargs
+        ).to_crs(self.crs)
+
+        # make sure MultiLineString are converted to LineString
+        gdf_obs = gdf_obs.explode().reset_index(drop=True)
+
+        if not gdf_obs.geometry.type.isin(["LineString"]).all():
+            raise ValueError("Observation lines must be of type LineString.")
+
+        if merge and name in self.geoms:
+            gdf0 = self._geoms.pop(name)
+            gdf_obs = gpd.GeoDataFrame(pd.concat([gdf_obs, gdf0], ignore_index=True))
+            self.logger.info(f"Adding new observation lines to existing ones.")
+
+        self.set_geoms(gdf_obs, name)
+        self.set_config(f"{name}file", f"sfincs.{name}")
+
     def setup_structures(
         self,
         structures: Union[str, Path, gpd.GeoDataFrame],
         stype: str,
+        dep: Union[str, Path, xr.DataArray] = None,
+        buffer: float = None,
         dz: float = None,
         merge: bool = True,
         **kwargs,
     ):
         """Setup thin dam or weir structures.
 
         Adds model layer (depending on `stype`):
@@ -1137,14 +1411,20 @@
         structures : str, Path
             Path, data source name, or geopandas object to structure line geometry file.
             The "name" (for thd and weir), "z" and "par1" (for weir only) variables are optional.
             For weirs: `dz` must be provided if gdf has no "z" column or ZLineString;
             "par1" defaults to 0.6 if gdf has no "par1" column.
         stype : {'thd', 'weir'}
             Structure type.
+        dep : str, Path, xr.DataArray, optional
+            Path, data source name, or xarray raster object ('elevtn') describing the depth in an
+            alternative resolution which is used for sampling the weir.
+        buffer : float, optional
+            If provided, describes the distance from the centerline to the foot of the structure.
+            This distance is supplied to the raster.sample as the window (wdw).
         merge : bool, optional
             If True, merge with existing'stype' structures, by default True.
         dz: float, optional
             If provided, for weir structures the z value is calculated from
             the model elevation (dep) plus dz.
         """
 
@@ -1153,28 +1433,52 @@
             structures, geom=self.region, **kwargs
         ).to_crs(self.crs)
 
         cols = {
             "thd": ["name", "geometry"],
             "weir": ["name", "z", "par1", "geometry"],
         }
-        assert stype in cols
+        assert stype in cols, f"stype must be one of {list(cols.keys())}"
         gdf = gdf_structures[
             [c for c in cols[stype] if c in gdf_structures.columns]
         ]  # keep relevant cols
 
         structs = utils.gdf2linestring(gdf)  # check if it parsed correct
         # sample zb values from dep file and set z = zb + dz
-        if stype == "weir" and dz is not None:
-            elv = self.grid["dep"]
+        if stype == "weir" and (dep is not None or dz is not None):
+            if dep is None or dep == "dep":
+                assert "dep" in self.grid, "dep layer not found"
+                elv = self.grid["dep"]
+            else:
+                elv = self.data_catalog.get_rasterdataset(
+                    dep, geom=self.region, buffer=5, variables=["elevtn"]
+                )
+
+            # calculate window size from buffer
+            if buffer is not None:
+                res = abs(elv.raster.res[0])
+                if elv.raster.crs.is_geographic:
+                    res = res * 111111.0
+                window_size = int(np.ceil(buffer / res))
+            else:
+                window_size = 0
+            self.logger.debug(f"Sampling elevation with window size {window_size}")
+
             structs_out = []
             for s in structs:
                 pnts = gpd.points_from_xy(x=s["x"], y=s["y"])
-                zb = elv.raster.sample(gpd.GeoDataFrame(geometry=pnts, crs=self.crs))
-                s["z"] = zb.values + float(dz)
+                zb = elv.raster.sample(
+                    gpd.GeoDataFrame(geometry=pnts, crs=self.crs), wdw=window_size
+                )
+                if zb.ndim > 1:
+                    zb = zb.max(axis=1)
+
+                s["z"] = zb.values
+                if dz is not None:
+                    s["z"] += float(dz)
                 structs_out.append(s)
             gdf = utils.linestring2gdf(structs_out, crs=self.crs)
         # Else function if you define elevation of weir
         elif stype == "weir" and np.any(["z" not in s for s in structs]):
             raise ValueError("Weir structure requires z values.")
         # combine with existing structures if present
         if merge and stype in self.geoms:
@@ -1182,14 +1486,96 @@
             gdf = gpd.GeoDataFrame(pd.concat([gdf, gdf0], ignore_index=True))
             self.logger.info(f"Adding {stype} structures to existing structures.")
 
         # set structures
         self.set_geoms(gdf, stype)
         self.set_config(f"{stype}file", f"sfincs.{stype}")
 
+    def setup_drainage_structures(
+        self,
+        structures: Union[str, Path, gpd.GeoDataFrame],
+        stype: str = "pump",
+        discharge: float = 0.0,
+        merge: bool = True,
+        **kwargs,
+    ):
+        """Setup drainage structures.
+
+        Adds model layer:
+        * **drn** geom: drainage pump or culvert
+
+        Parameters
+        ----------
+        structures : str, Path
+            Path, data source name, or geopandas object to structure line geometry file.
+            The line should consist of only 2 points (else first and last points are used), ordered from up to downstream.
+            The "type" (1 for pump and 2 for culvert), "par1" ("discharge" also accepted) variables are optional.
+            If "type" or "par1" are not provided, they are based on stype or discharge arguments.
+        stype : {'pump', 'culvert'}, optional
+            Structure type, by default "pump". stype is converted to integer "type" to match with SFINCS expectations.
+        discharge : float, optional
+            Discharge of the structure, by default 0.0. For culverts, this is the maximum discharge,
+            since actual discharge depends on waterlevel gradient
+        merge : bool, optional
+            If True, merge with existing drainage structures, by default True.
+        """
+
+        stype = stype.lower()
+        svalues = {"pump": 1, "culvert": 2}
+        if stype not in svalues:
+            raise ValueError('stype must be one of "pump", "culvert"')
+        svalue = svalues[stype]
+
+        # read, clip and reproject
+        gdf_structures = self.data_catalog.get_geodataframe(
+            structures, geom=self.region, **kwargs
+        ).to_crs(self.crs)
+
+        # check if type (int) is present in gdf, else overwrite from args
+        # TODO also add check if type is interger?
+        if "type" not in gdf_structures:
+            gdf_structures["type"] = svalue
+        # if discharge is provided, rename to par1
+        if "discharge" in gdf_structures:
+            gdf_structures = gdf_structures.rename(columns={"discharge": "par1"})
+
+        # add par1, par2, par3, par4, par5 if not present
+        # NOTE only par1 is used in the model
+        if "par1" not in gdf_structures:
+            gdf_structures["par1"] = discharge
+        if "par2" not in gdf_structures:
+            gdf_structures["par2"] = 0
+        if "par3" not in gdf_structures:
+            gdf_structures["par3"] = 0
+        if "par4" not in gdf_structures:
+            gdf_structures["par4"] = 0
+        if "par5" not in gdf_structures:
+            gdf_structures["par5"] = 0
+
+        # multi to single lines
+        lines = gdf_structures.explode(column="geometry").reset_index(drop=True)
+        # get start [0] and end [1] points
+        endpoints = lines.boundary.explode().unstack()
+        # merge start and end points into a single linestring
+        gdf_structures["geometry"] = endpoints.apply(
+            lambda x: LineString(x.values.tolist()), axis=1
+        )
+
+        # combine with existing structures if present
+        if merge and "drn" in self.geoms:
+            gdf0 = self._geoms.pop("drn")
+            gdf_structures = gpd.GeoDataFrame(
+                pd.concat([gdf_structures, gdf0], ignore_index=True)
+            )
+            self.logger.info(f"Adding {stype} structures to existing structures.")
+
+        # set structures
+        self.set_geoms(gdf_structures, "drn")
+        self.set_config("drnfile", f"sfincs.drn")
+
     ### FORCING
     def set_forcing_1d(
         self,
         df_ts: pd.DataFrame = None,
         gdf_locs: gpd.GeoDataFrame = None,
         name: str = "bzs",
         merge: bool = True,
@@ -1327,14 +1713,15 @@
         ----------
         geodataset: str, Path, xr.Dataset, optional
             Path, data source name, or xarray data object for geospatial point timeseries.
         timeseries: str, Path, pd.DataFrame, optional
             Path, data source name, or pandas data object for tabular timeseries.
         locations: str, Path, gpd.GeoDataFrame, optional
             Path, data source name, or geopandas object for bnd point locations.
+            It should contain a 'index' column matching the column names in `timeseries`.
         offset: str, Path, xr.Dataset, float, optional
             Path, data source name, constant value or xarray raster data for gridded offset
             between vertical reference of elevation and waterlevel data,
             The offset is added to the waterlevel data.
         buffer: float, optional
             Buffer [m] around model water level boundary cells to select waterlevel gauges,
             by default 5 km.
@@ -1370,45 +1757,47 @@
                 timeseries,
                 time_tuple=(tstart, tstop),
                 # kwargs below only applied if timeseries not in data catalog
                 parse_dates=True,
                 index_col=0,
             )
             df_ts.columns = df_ts.columns.map(int)  # parse column names to integers
-        else:
-            raise ValueError("Either geodataset or timeseries must be provided")
 
-        # optionally read location data (if not already read from geodataset)
+        # read location data (if not already read from geodataset)
         if gdf_locs is None and locations is not None:
             gdf_locs = self.data_catalog.get_geodataframe(
                 locations, geom=region, buffer=buffer, crs=self.crs
             ).to_crs(self.crs)
+            if "index" in gdf_locs.columns:
+                gdf_locs = gdf_locs.set_index("index")
         elif gdf_locs is None and "bzs" in self.forcing:
             gdf_locs = self.forcing["bzs"].vector.to_gdf()
         elif gdf_locs is None:
             raise ValueError("No waterlevel boundary (bnd) points provided.")
 
         # optionally read offset data and correct df_ts
         if offset is not None and gdf_locs is not None:
             if isinstance(offset, (float, int)):
                 df_ts += offset
             else:
                 da_offset = self.data_catalog.get_rasterdataset(
-                    offset, geom=self.region, buffer=5
+                    offset,
+                    bbox=self.mask.raster.transform_bounds(4326),
+                    buffer=5,
                 )
                 offset_pnts = da_offset.raster.sample(gdf_locs)
                 df_offset = offset_pnts.to_pandas().reindex(df_ts.columns).fillna(0)
                 df_ts = df_ts + df_offset
                 offset = offset_pnts.mean().values
             self.logger.debug(
                 f"waterlevel forcing: applied offset (avg: {offset:+.2f})"
             )
 
         # set/ update forcing
-        self.set_forcing_1d(df_ts, gdf_locs, name="bzs", merge=merge)
+        self.set_forcing_1d(df_ts=df_ts, gdf_locs=gdf_locs, name="bzs", merge=merge)
 
     def setup_waterlevel_bnd_from_mask(
         self,
         distance: float = 1e4,
         merge: bool = True,
     ):
         """Setup waterlevel boundary (bnd) points along model waterlevel boundary (msk=2).
@@ -1447,15 +1836,20 @@
         # create geodataframe with points
         gdf = gpd.GeoDataFrame(geometry=gpd.points_from_xy(*zip(*points)), crs=self.crs)
 
         # set waterlevel boundary
         self.set_forcing_1d(gdf_locs=gdf, name="bzs", merge=merge)
 
     def setup_discharge_forcing(
-        self, geodataset=None, timeseries=None, locations=None, merge=True
+        self,
+        geodataset=None,
+        timeseries=None,
+        locations=None,
+        merge=True,
+        buffer: float = None,
     ):
         """Setup discharge forcing.
 
         Discharge timeseries are read from a `geodataset` (geospatial point timeseries)
         or a tabular `timeseries` dataframe. At least one of these must be provided.
 
         The tabular timeseries data is combined with `locations` if provided,
@@ -1470,29 +1864,37 @@
         ----------
         geodataset: str, Path, xr.Dataset, optional
             Path, data source name, or xarray data object for geospatial point timeseries.
         timeseries: str, Path, pd.DataFrame, optional
             Path, data source name, or pandas data object for tabular timeseries.
         locations: str, Path, gpd.GeoDataFrame, optional
             Path, data source name, or geopandas object for bnd point locations.
+            It should contain a 'index' column matching the column names in `timeseries`.
         merge : bool, optional
             If True, merge with existing forcing data, by default True.
+        buffer: float, optional
+            Buffer [m] around model boundary within the model region
+            select discharge gauges, by default None.
 
         See Also
         --------
         setup_river_inflow
         """
         gdf_locs, df_ts = None, None
         tstart, tstop = self.get_model_time()  # model time
+        # buffer
+        region = self.region
+        if buffer is not None:  # TODO this assumes the model crs is projected
+            region = region.boundary.buffer(buffer).clip(self.region)
         # read waterlevel data from geodataset or geodataframe
         if geodataset is not None:
             # read and clip data in time & space
             da = self.data_catalog.get_geodataset(
                 geodataset,
-                geom=self.region,
+                geom=region,
                 variables=["discharge"],
                 time_tuple=(tstart, tstop),
                 crs=self.crs,
             )
             df_ts = da.transpose(..., da.vector.index_dim).to_pandas()
             gdf_locs = da.vector.to_gdf()
         elif timeseries is not None:
@@ -1500,29 +1902,29 @@
                 timeseries,
                 time_tuple=(tstart, tstop),
                 # kwargs below only applied if timeseries not in data catalog
                 parse_dates=True,
                 index_col=0,
             )
             df_ts.columns = df_ts.columns.map(int)  # parse column names to integers
-        else:
-            raise ValueError("Either geodataset or timeseries must be provided")
 
-        # optionally read location data (if not already read from geodataset)
+        # read location data (if not already read from geodataset)
         if gdf_locs is None and locations is not None:
             gdf_locs = self.data_catalog.get_geodataframe(
-                locations, geom=self.region, crs=self.crs
+                locations, geom=region, crs=self.crs
             ).to_crs(self.crs)
+            if "index" in gdf_locs.columns:
+                gdf_locs = gdf_locs.set_index("index")
         elif gdf_locs is None and "dis" in self.forcing:
             gdf_locs = self.forcing["dis"].vector.to_gdf()
         elif gdf_locs is None:
             raise ValueError("No discharge boundary (src) points provided.")
 
         # set/ update forcing
-        self.set_forcing_1d(df_ts, gdf_locs, name="dis", merge=merge)
+        self.set_forcing_1d(df_ts=df_ts, gdf_locs=gdf_locs, name="dis", merge=merge)
 
     def setup_discharge_forcing_from_grid(
         self,
         discharge,
         locations=None,
         uparea=None,
         wdw=1,
@@ -1582,23 +1984,26 @@
             gdf = self.forcing["dis"].vector.to_gdf()
         else:
             raise ValueError("No discharge boundary (src) points provided.")
 
         # read data
         ds = self.data_catalog.get_rasterdataset(
             discharge,
-            geom=self.region,
+            bbox=self.mask.raster.transform_bounds(4326),
             buffer=2,
             time_tuple=self.get_model_time(),  # model time
             variables=["discharge"],
             single_var_as_array=False,
         )
         if uparea is not None and "uparea" in gdf.columns:
             da_upa = self.data_catalog.get_rasterdataset(
-                uparea, geom=self.region, buffer=2, variables=["uparea"]
+                uparea,
+                bbox=self.mask.raster.transform_bounds(4326),
+                buffer=2,
+                variables=["uparea"],
             )
             # make sure ds and da_upa align
             ds["uparea"] = da_upa.raster.reproject_like(ds, method="nearest")
         elif "uparea" not in gdf.columns:
             self.logger.warning('No "uparea" column found in location data.')
 
         # TODO use hydromt core method
@@ -1617,15 +2022,15 @@
         df_q = da_q.transpose("time", ...).to_pandas()
         # update forcing
         self.set_forcing_1d(df_ts=df_q, gdf_locs=gdf, name="dis")
         # keep snapped locations
         self.set_geoms(ds_snapped.vector.to_gdf(), "src_snapped")
 
     def setup_precip_forcing_from_grid(
-        self, precip=None, dst_res=None, aggregate=False, **kwargs
+        self, precip, dst_res=None, aggregate=False, **kwargs
     ):
         """Setup precipitation forcing from a gridded spatially varying data source.
 
         If aggregate is True, spatially uniform precipitation forcing is added to
         the model based on the mean precipitation over the model domain.
         If aggregate is False, distributed precipitation is added to the model as netcdf file.
         The data is reprojected to the model CRS (and destination resolution `dst_res` if provided).
@@ -1650,15 +2055,15 @@
             Method to aggregate distributed input precipitation data. If True, mean
             aggregation is used, if False (default) the data is not aggregated and
             spatially distributed precipitation is returned.
         """
         # get data for model domain and config time range
         precip = self.data_catalog.get_rasterdataset(
             precip,
-            geom=self.region,
+            bbox=self.mask.raster.transform_bounds(4326),
             buffer=2,
             time_tuple=self.get_model_time(),
             variables=["precip"],
         )
 
         # aggregate or reproject in space
         if aggregate:
@@ -1676,58 +2081,238 @@
             kwargs0.update(kwargs)
             meth = kwargs0["method"]
             self.logger.debug(f"Resample precip using {meth}.")
             precip_out = precip.raster.reproject(
                 dst_crs=self.crs, dst_res=dst_res, **kwargs
             ).fillna(0)
 
-            # resample in time
-            precip_out = hydromt.workflows.resample_time(
-                precip_out,
-                freq=pd.to_timedelta("1H"),
-                conserve_mass=True,
-                upsampling="bfill",
-                downsampling="sum",
-                logger=self.logger,
-            ).rename("precip")
+            # only resample in time if freq < 1H, else keep input values
+            if da_to_timedelta(precip_out) < pd.to_timedelta("1H"):
+                precip_out = hydromt.workflows.resample_time(
+                    precip_out,
+                    freq=pd.to_timedelta("1H"),
+                    conserve_mass=True,
+                    upsampling="bfill",
+                    downsampling="sum",
+                    logger=self.logger,
+                )
+            precip_out = precip_out.rename("precip_2d")
 
             # add to forcing
-            self.set_forcing(precip_out, name="precip")
+            self.set_forcing(precip_out, name="precip_2d")
 
-    def setup_precip_forcing(self, timeseries):
+    def setup_precip_forcing(self, timeseries=None, magnitude=None):
         """Setup spatially uniform precipitation forcing (precip).
 
         Adds model layers:
 
         * **precipfile** forcing: uniform precipitation [mm/hr]
 
         Parameters
         ----------
         timeseries, str, Path
             Path to tabulated timeseries csv file with time index in first column
             and location IDs in the first row,
             see :py:meth:`hydromt.open_timeseries_from_table`, for details.
             Note: tabulated timeseries files cannot yet be set through the data_catalog yml file.
+        magnitude: float
+            Precipitation magnitude [mm/hr] to use if no timeseries is provided.
         """
         tstart, tstop = self.get_model_time()
-        df_ts = self.data_catalog.get_dataframe(
-            timeseries,
-            time_tuple=(tstart, tstop),
-            # kwargs below only applied if timeseries not in data catalog
-            parse_dates=True,
-            index_col=0,
-        )
+        if timeseries is not None:
+            df_ts = self.data_catalog.get_dataframe(
+                timeseries,
+                time_tuple=(tstart, tstop),
+                # kwargs below only applied if timeseries not in data catalog
+                parse_dates=True,
+                index_col=0,
+            )
+        elif magnitude is not None:
+            times = pd.date_range(*self.get_model_time(), freq="10T")
+            df_ts = pd.DataFrame(
+                index=times, data=np.full((len(times), 1), magnitude, dtype=float)
+            )
+        else:
+            raise ValueError("Either timeseries or magnitude must be provided")
+
         if isinstance(df_ts, pd.DataFrame):
             df_ts = df_ts.squeeze()
         if not isinstance(df_ts, pd.Series):
             raise ValueError("df_ts must be a pandas.Series")
         df_ts.name = "precip"
         df_ts.index.name = "time"
         self.set_forcing(df_ts.to_xarray(), name="precip")
 
+    def setup_pressure_forcing_from_grid(
+        self, press, dst_res=None, fill_value=101325, **kwargs
+    ):
+        """Setup pressure forcing from a gridded spatially varying data source.
+
+        Adds one model layer:
+
+        * **netampfile** forcing: distributed barometric pressure [Pa]
+
+        Parameters
+        ----------
+        press, str, Path, xr.Dataset, xr.DataArray
+            Path to pressure rasterdataset netcdf file or xarray dataset.
+
+            * Required variables: ['press' (Pa)]
+            * Required coordinates: ['time', 'y', 'x']
+
+        dst_res: float
+            output resolution (m), by default None and computed from source data.
+
+        fill_value: float
+            value to use when no data is available.
+            Standard atmospheric pressure (101325 Pa) is used if no value is given.
+        """
+        # get data for model domain and config time range
+        press = self.data_catalog.get_rasterdataset(
+            press,
+            geom=self.region,
+            buffer=2,
+            time_tuple=self.get_model_time(),
+            variables=["press"],
+        )
+
+        # reproject to model utm crs
+        # NOTE: currently SFINCS errors (stack overflow) on large files,
+        # downscaling to model grid is not recommended
+        kwargs0 = dict(align=dst_res is not None, method="nearest_index")
+        kwargs0.update(kwargs)
+        meth = kwargs0["method"]
+        self.logger.debug(f"Resample pressure using {meth}.")
+        press_out = press.raster.reproject(
+            dst_crs=self.crs, dst_res=dst_res, **kwargs
+        ).fillna(fill_value)
+
+        # only resample in time if freq < 1H, else keep input values
+        if da_to_timedelta(press_out) < pd.to_timedelta("1H"):
+            press_out = hydromt.workflows.resample_time(
+                press_out,
+                freq=pd.to_timedelta("1H"),
+                conserve_mass=False,
+                upsampling="interpolate",
+                downsampling="interpolate",
+                logger=self.logger,
+            )
+
+        press_out = press_out.rename("press_2d")
+
+        # add to forcing
+        self.set_forcing(press_out, name="press_2d")
+
+    def setup_wind_forcing_from_grid(self, wind, dst_res=None, **kwargs):
+        """Setup pressure forcing from a gridded spatially varying data source.
+
+        Adds one model layer:
+
+        * **netamuamv** forcing: distributed wind [m/s]
+
+        Parameters
+        ----------
+        wind, str, Path, xr.Dataset
+            Path to wind rasterdataset (including eastward and northward components) netcdf file or xarray dataset.
+
+            * Required variables: ['wind_u' (m/s), 'wind_v' (m/s)]
+            * Required coordinates: ['time', 'y', 'x']
+
+        dst_res: float
+            output resolution (m), by default None and computed from source data.
+        """
+        # get data for model domain and config time range
+        wind = self.data_catalog.get_rasterdataset(
+            wind,
+            geom=self.region,
+            buffer=2,
+            time_tuple=self.get_model_time(),
+            variables=["wind_u", "wind_v"],
+        )
+
+        # reproject to model utm crs
+        # NOTE: currently SFINCS errors (stack overflow) on large files,
+        # downscaling to model grid is not recommended
+        kwargs0 = dict(align=dst_res is not None, method="nearest_index")
+        kwargs0.update(kwargs)
+        meth = kwargs0["method"]
+        self.logger.debug(f"Resample wind using {meth}.")
+
+        wind = wind.raster.reproject(
+            dst_crs=self.crs, dst_res=dst_res, **kwargs
+        ).fillna(0)
+
+        # only resample in time if freq < 1H, else keep input values
+        if da_to_timedelta(wind) < pd.to_timedelta("1H"):
+            wind_out = xr.Dataset()
+            # resample in time
+            for var in wind.data_vars:
+                wind_out[var] = hydromt.workflows.resample_time(
+                    wind[var],
+                    freq=pd.to_timedelta("1H"),
+                    conserve_mass=False,
+                    upsampling="interpolate",
+                    downsampling="interpolate",
+                    logger=self.logger,
+                )
+        else:
+            wind_out = wind
+
+        # add to forcing
+        self.set_forcing(wind_out, name="wind_2d")
+
+    def setup_wind_forcing(self, timeseries=None, magnitude=None, direction=None):
+        """Setup spatially uniform wind forcing (wind).
+
+        Adds model layers:
+
+        * **windfile** forcing: uniform wind magnitude [m/s] and direction [deg]
+
+        Parameters
+        ----------
+        timeseries, str, Path
+            Path to tabulated timeseries csv file with time index in first column,
+            magnitude in second column and direction in third column
+            see :py:meth:`hydromt.open_timeseries_from_table`, for details.
+            Note: tabulated timeseries files cannot yet be set through the data_catalog yml file.
+        magnitude: float
+            Magnitude of the wind [m/s]
+        direction: float
+            Direction where the wind is coming from [deg], e.g. 0 is north, 90 is east, etc.
+        """
+        tstart, tstop = self.get_model_time()
+        if timeseries is not None:
+            df_ts = self.data_catalog.get_dataframe(
+                timeseries,
+                time_tuple=(tstart, tstop),
+                # kwargs below only applied if timeseries not in data catalog
+                parse_dates=True,
+                index_col=0,
+            )
+        elif magnitude is not None and direction is not None:
+            df_ts = pd.DataFrame(
+                index=pd.date_range(*self.get_model_time(), periods=2),
+                data=np.array([[magnitude, direction], [magnitude, direction]]),
+                columns=["mag", "dir"],
+            )
+        else:
+            raise ValueError(
+                "Either timeseries or magnitude and direction must be provided"
+            )
+
+        df_ts.name = "wnd"
+        df_ts.index.name = "time"
+        df_ts.columns.name = "index"
+        da = xr.DataArray(
+            df_ts.values,
+            dims=("time", "index"),
+            coords={"time": df_ts.index, "index": ["mag", "dir"]},
+        )
+        self.set_forcing(da, name="wnd")
+
     def setup_tiles(
         self,
         path: Union[str, Path] = None,
         region: dict = None,
         datasets_dep: List[dict] = [],
         zoom_range: Union[int, List[int]] = [0, 13],
         z_range: List[int] = [-20000.0, 20000.0],
@@ -1830,15 +2415,15 @@
                 fmt=fmt,
             )
 
     # Plotting
     def plot_forcing(self, fn_out=None, **kwargs):
         """Plot model timeseries forcing.
 
-        For distributed forcing a spatial avarage is plotted.
+        For distributed forcing a spatial avarage, minimum or maximum is plotted.
 
         Parameters
         ----------
         fn_out: str
             Path to output figure file.
             If a basename is given it is saved to <model_root>/figs/<fn_out>
             If None, no file is saved.
@@ -2000,15 +2585,15 @@
         self.write_subgrid()
         self.write_geoms()
         self.write_forcing()
         self.write_states()
         # config last; might be udpated when writing maps, states or forcing
         self.write_config()
         # write data catalog with used data sources
-        # self.write_data_catalog()  # new in hydromt v0.4.4
+        self.write_data_catalog()  # new in hydromt v0.4.4
 
     def read_grid(self, data_vars: Union[List, str] = None) -> None:
         """Read SFINCS binary grid files and save to `grid` attribute.
         Filenames are taken from the `config` attribute (i.e. input file).
 
         Parameters
         ----------
@@ -2135,33 +2720,35 @@
                 self.set_config(f"sbgfile", f"sfincs.sbg")
             fn = self.get_config(f"sbgfile", abs_path=True)
             self.reggrid.subgrid.save(file_name=fn, mask=self.mask)
 
     def read_geoms(self):
         """Read geometry files and save to `geoms` attribute.
         Known geometry files mentioned in the sfincs.inp configuration file are read,
-        including: bnd/src/obs xy files and thd/weir structure files.
+        including: bnd/src/obs xy(n) files, thd/weir structure files and drn drainage structure files.
 
         If other geojson files are present in a "gis" subfolder folder, those are read as well.
         """
         self._assert_read_mode
         # read _GEOMS model files
         for gname in self._GEOMS.values():
             if f"{gname}file" in self.config:
                 fn = self.get_config(f"{gname}file", abs_path=True)
                 if fn is None:
                     continue
                 elif not isfile(fn):
                     self.logger.warning(f"{gname}file not found at {fn}")
                     continue
-                if gname in ["thd", "weir"]:
+                if gname in ["thd", "weir", "crs"]:
                     struct = utils.read_geoms(fn)
                     gdf = utils.linestring2gdf(struct, crs=self.crs)
                 elif gname == "obs":
                     gdf = utils.read_xyn(fn, crs=self.crs)
+                elif gname == "drn":
+                    gdf = utils.read_drn(fn, crs=self.crs)
                 else:
                     gdf = utils.read_xy(fn, crs=self.crs)
                 self.set_geoms(gdf, name=gname)
         # read additional geojson files from gis directory
         for fn in glob.glob(join(self.root, "gis", "*.geojson")):
             name = basename(fn).replace(".geojson", "")
             gnames = [f[1] for f in self._FORCING_1D.values() if f[1] is not None]
@@ -2192,19 +2779,21 @@
                 dvars = [name for name in data_vars if name in self._GEOMS.values()]
             self.logger.info("Write geom files")
             for gname, gdf in self.geoms.items():
                 if gname in dvars:
                     if f"{gname}file" not in self.config:
                         self.set_config(f"{gname}file", f"sfincs.{gname}")
                     fn = self.get_config(f"{gname}file", abs_path=True)
-                    if gname in ["thd", "weir"]:
+                    if gname in ["thd", "weir", "crs"]:
                         struct = utils.gdf2linestring(gdf)
                         utils.write_geoms(fn, struct, stype=gname)
                     elif gname == "obs":
                         utils.write_xyn(fn, gdf, crs=self.crs)
+                    elif gname == "drn":
+                        utils.write_drn(fn, gdf)
                     else:
                         utils.write_xy(fn, gdf, fmt="%8.2f")
 
             # NOTE: all geoms are written to geojson files in a "gis" subfolder
             if self._write_gis:
                 self.write_vector(variables=["geoms"])
 
@@ -2250,25 +2839,30 @@
             if xy_name is not None:
                 xy_fn = self.get_config(f"{xy_name}file", abs_path=True)
                 if xy_fn is None or not isfile(xy_fn):
                     if xy_fn is not None:
                         self.logger.warning(f"{xy_name}file not found at {xy_fn}")
                 else:
                     gdf = utils.read_xy(xy_fn, crs=self.crs)
-                    # read attribute data from gis files
+                    # read attribute data from gis files; merge based on index
                     gis_fn = join(self.root, "gis", f"{xy_name}.geojson")
                     if isfile(gis_fn):
                         gdf1 = gpd.read_file(gis_fn)
                         if "index" in gdf1.columns:
                             gdf1 = gdf1.set_index("index")
-                            gdf.index = gdf1.index.values
-                            ds = ds.assign_coords(index=gdf1.index.values)
-                        if np.any(gdf1.columns != "geometry"):
-                            gdf = gpd.sjoin(gdf, gdf1, how="left")[gdf1.columns]
-                    # set locations as coordinates dataset
+                        if not np.all(np.isin(gdf.index, gdf1.index)):
+                            self.logger.warning(
+                                f"Index in {xy_name}file does not match {gis_fn}"
+                            )
+                        else:
+                            for col in gdf1.columns:
+                                if col not in gdf.columns:
+                                    gdf[col] = gdf1.loc[gdf.index, col]
+                    # set locations and attributes as coordinates of dataset
+                    ds = ds.assign_coords(index=gdf.index.values)
                     ds = GeoDataset.from_gdf(gdf, ds, index_dim="index")
             # save in self.forcing
             if len(ds) > 1:
                 # keep wave forcing together
                 self.set_forcing(ds, name=name, split_dataset=False)
             elif len(ds) > 0:
                 self.set_forcing(ds, split_dataset=True)
@@ -2370,15 +2964,15 @@
                 if (
                     name in self._FORCING_1D
                     and f"{self._FORCING_1D[name][1]}file" in self.config
                 ):
                     continue  # timeseries + xy file already written
                 fname, rename = self._FORCING_NET[name]
                 # combine variables and rename to output names
-                rename = {v: k for k, v in rename.items() if v in ds}
+                rename = {v: k for k, v in rename.items() if v in self.forcing}
                 if len(rename) == 0:
                     continue
                 ds = xr.merge([self.forcing[v] for v in rename.keys()]).rename(rename)
                 # get filename from config
                 if f"{fname}file" not in self.config:
                     self.set_config(f"{fname}file", f"{name}.nc")
                 fn = self.get_config(f"{fname}file", abs_path=True)
@@ -2640,50 +3234,43 @@
                             f"Variable {attr}.{name} could not be written to vector file."
                         )
                         pass
                 gdf.to_file(join(root, f"{name}.geojson"), **kwargs)
 
     ## model configuration
 
-    def read_config(self, config_fn: str = "sfincs.inp", epsg: int = None) -> None:
+    def read_config(self, config_fn: str = None, epsg: int = None) -> None:
         """Parse config from SFINCS input file.
-        If in write-only mode the config is initialized with default settings.
+        If in write-only mode the config is initialized with default settings
+        unless a path to a template config file is provided.
 
         Parameters
         ----------
         config_fn: str
-            Filename of config file, by default "sfincs.inp".
-            If in a different folder than the model root, the root is updated.
+            Filename of config file, by default None.
         epsg: int
-            EPSG code of the model CRS. Only used if missing in the SFINCS input file, by default None.
+            EPSG code of the model CRS. Only used if missing in the SFINCS input file,
+            by default None.
         """
         inp = SfincsInput()  # initialize with defaults
-        if self._read:  # in read-only or append mode, try reading config_fn
-            if not isfile(config_fn) and not isabs(config_fn) and self._root:
-                # path relative to self.root
+        if config_fn is not None or self._read:
+            if config_fn is None:  # read from default location
+                config_fn = self._config_fn
+            if not isabs(config_fn) and self._root:  # read from model root
                 config_fn = abspath(join(self.root, config_fn))
-            elif isfile(config_fn) and abspath(dirname(config_fn)) != self._root:
-                # new root
-                mode = (
-                    "r+"
-                    if self._write and self._read
-                    else ("w" if self._write else "r")
-                )
-                root = abspath(dirname(config_fn))
-                self.logger.warning(f"updating the model root to: {root}")
-                self.set_root(root=root, mode=mode)
-            else:
+            if not isfile(config_fn):
                 raise IOError(f"SFINCS input file not found {config_fn}")
-            # read config_fn
+            # read inp file
             inp.read(inp_fn=config_fn)
         # overwrite / initialize config attribute
         self._config = inp.to_dict()
         if epsg is not None and "epsg" not in self.config:
-            self.config.update(epsg=epsg)
-        self.update_grid_from_config()  # update grid properties based on sfincs.inp
+            self.set_config("epsg", int(epsg))
+        # update grid properties based on sfincs.inp
+        self.update_grid_from_config()
 
     def write_config(self, config_fn: str = "sfincs.inp"):
         """Write config to <root/config_fn>"""
         self._assert_write_mode
         if not isabs(config_fn) and self._root:
             config_fn = join(self.root, config_fn)
 
@@ -2727,142 +3314,224 @@
     def get_model_time(self):
         """Return (tstart, tstop) tuple with parsed model start and end time"""
         tstart = utils.parse_datetime(self.config["tstart"])
         tstop = utils.parse_datetime(self.config["tstop"])
         return tstart, tstop
 
     ## helper method
-
     def _parse_datasets_dep(self, datasets_dep, res):
-        """Parse filenames or paths of Datasets in list of dictionaries datasets_dep into xr.DataArray and gdf.GeoDataFrames:
+        """Parse filenames or paths of Datasets in list of dictionaries datasets_dep
+        into xr.DataArray and gdf.GeoDataFrames:
+
         * "elevtn" is parsed into da (xr.DataArray)
         * "offset" is parsed into da_offset (xr.DataArray)
         * "mask" is parsed into gdf (gpd.GeoDataFrame)
 
         Parameters
         ----------
         datasets_dep : List[dict]
-            List of dictionaries with topobathy data, each containing a dataset name or Path (dep) and optional merge arguments.
+            List of dictionaries with topobathy data, each containing a dataset name or
+            Path (dep) and optional merge arguments.
         res : float
-            Resolution of the model grid in meters. Used to obtain the correct zoom level of the depth datasets.
+            Resolution of the model grid in meters. Used to obtain the correct zoom
+            level of the depth datasets.
         """
         parse_keys = ["elevtn", "offset", "mask", "da"]
         copy_keys = ["zmin", "zmax", "reproj_method", "merge_method"]
 
         datasets_out = []
         for dataset in datasets_dep:
             dd = {}
             # read in depth datasets; replace dep (source name; filename or xr.DataArray)
             if "elevtn" in dataset or "da" in dataset:
                 try:
                     da_elv = self.data_catalog.get_rasterdataset(
                         dataset.get("elevtn", dataset.get("da")),
-                        geom=self.mask.raster.box,
+                        bbox=self.mask.raster.transform_bounds(4326),
                         buffer=10,
                         variables=["elevtn"],
                         zoom_level=(res, "meter"),
                     )
-                    dd.update({"da": da_elv})
-                except:
+                # TODO remove ValueError after fix in hydromt core
+                except (IndexError, ValueError):
                     data_name = dataset.get("elevtn")
-                    self.logger.warning(
-                        f"{data_name} not used; probably because all the data is outside of the mask."
-                    )
+                    self.logger.warning(f"No data in domain for {data_name}, skipped.")
                     continue
+                dd.update({"da": da_elv})
             else:
                 raise ValueError(
                     "No 'elevtn' (topobathy) dataset provided in datasets_dep."
                 )
 
             # read offset filenames
             # NOTE offsets can be xr.DataArrays and floats
             if "offset" in dataset and not isinstance(dataset["offset"], (float, int)):
                 da_offset = self.data_catalog.get_rasterdataset(
                     dataset.get("offset"),
-                    geom=self.mask.raster.box,
-                    buffer=20,
+                    bbox=self.mask.raster.transform_bounds(4326),
+                    buffer=10,
                 )
                 dd.update({"offset": da_offset})
 
             # read geodataframes describing valid areas
             if "mask" in dataset:
                 gdf_valid = self.data_catalog.get_geodataframe(
                     path_or_key=dataset.get("mask"),
-                    geom=self.mask.raster.box,
+                    bbox=self.mask.raster.transform_bounds(4326),
                 )
                 dd.update({"gdf_valid": gdf_valid})
 
             # copy remaining keys
             for key, value in dataset.items():
                 if key in copy_keys and key not in dd:
                     dd.update({key: value})
                 elif key not in copy_keys + parse_keys:
                     self.logger.warning(f"Unknown key {key} in datasets_dep. Ignoring.")
             datasets_out.append(dd)
 
         return datasets_out
 
     def _parse_datasets_rgh(self, datasets_rgh):
-        """Parse filenames or paths of Datasets in list of dictionaries datasets_rgh into xr.DataArrays and gdf.GeoDataFrames:
+        """Parse filenames or paths of Datasets in list of dictionaries datasets_rgh
+        into xr.DataArrays and gdf.GeoDataFrames:
+
         * "manning" is parsed into da (xr.DataArray)
-        * "lulc" is parsed into da (xr.DataArray) using reclassify table in "reclass_table"
+        * "lulc" is parsed into da (xr.DataArray) using reclass table in "reclass_table"
         * "mask" is parsed into gdf_valid (gpd.GeoDataFrame)
 
         Parameters
         ----------
         datasets_rgh : List[dict], optional
-            List of dictionaries with Manning's n datasets. Each dictionary should at least contain one of the following:
+            List of dictionaries with Manning's n datasets. Each dictionary should at
+            least contain one of the following:
             * (1) manning: filename (or Path) of gridded data with manning values
-            * (2) lulc (and reclass_table) :a combination of a filename of gridded landuse/landcover and a reclassify table.
+            * (2) lulc (and reclass_table): a combination of a filename of gridded
+                  landuse/landcover and a reclassify table.
             In additon, optional merge arguments can be provided e.g.: merge_method, mask
         """
         parse_keys = ["manning", "lulc", "reclass_table", "mask", "da"]
         copy_keys = ["reproj_method", "merge_method"]
 
         datasets_out = []
         for dataset in datasets_rgh:
             dd = {}
 
             if "manning" in dataset or "da" in dataset:
                 da_man = self.data_catalog.get_rasterdataset(
                     dataset.get("manning", dataset.get("da")),
-                    geom=self.mask.raster.box,
+                    bbox=self.mask.raster.transform_bounds(4326),
                     buffer=10,
                 )
                 dd.update({"da": da_man})
             elif "lulc" in dataset:
                 # landuse/landcover should always be combined with mapping
                 lulc = dataset.get("lulc")
                 reclass_table = dataset.get("reclass_table", None)
                 if reclass_table is None and isinstance(lulc, str):
                     reclass_table = join(DATADIR, "lulc", f"{lulc}_mapping.csv")
-                if not os.path.isfile(reclass_table) and isinstance(lulc, str):
+                if reclass_table is None:
                     raise IOError(
                         f"Manning roughness mapping file not found: {reclass_table}"
                     )
                 da_lulc = self.data_catalog.get_rasterdataset(
-                    lulc, geom=self.mask.raster.box, buffer=10, variables=["lulc"]
+                    lulc,
+                    bbox=self.mask.raster.transform_bounds(4326),
+                    buffer=10,
+                    variables=["lulc"],
                 )
                 df_map = self.data_catalog.get_dataframe(reclass_table, index_col=0)
                 # reclassify
                 da_man = da_lulc.raster.reclassify(df_map[["N"]])["N"]
                 dd.update({"da": da_man})
             else:
                 raise ValueError("No 'manning' dataset provided in datasets_rgh.")
 
             # read geodataframes describing valid areas
             if "mask" in dataset:
                 gdf_valid = self.data_catalog.get_geodataframe(
                     path_or_key=dataset.get("mask"),
-                    geom=self.mask.raster.box,
+                    bbox=self.mask.raster.transform_bounds(4326),
                 )
                 dd.update({"gdf_valid": gdf_valid})
 
             # copy remaining keys
             for key, value in dataset.items():
                 if key in copy_keys and key not in dd:
                     dd.update({key: value})
                 elif key not in copy_keys + parse_keys:
                     self.logger.warning(f"Unknown key {key} in datasets_rgh. Ignoring.")
             datasets_out.append(dd)
 
         return datasets_out
+
+    def _parse_datasets_riv(self, datasets_riv):
+        """Parse filenames or paths of Datasets in list of dictionaries
+        datasets_riv into xr.DataArrays and gdf.GeoDataFrames:
+
+        see SfincsModel.setup_subgrid for details
+        """
+        # option 1: rectangular river cross-sections based on river centerline
+        # depth/bedlevel, manning attributes are specified on the river centerline
+        # TODO: make this work with LineStringZ geometries for bedlevel
+        # the width is either specified on the river centerline or river mask
+        # option 2: (TODO): irregular river cross-sections
+        # cross-sections are specified as a series of points (river_crosssections)
+        parse_keys = [
+            "centerlines",
+            "mask",
+            "gdf_riv",
+            "gdf_riv_mask",
+        ]
+        copy_keys = []
+        attrs = ["rivwth", "rivdph", "rivbed", "manning"]
+
+        datasets_out = []
+        for dataset in datasets_riv:
+            dd = {}
+
+            # parse rivers
+            if "centerlines" in dataset:
+                rivers = dataset.get("centerlines")
+                if isinstance(rivers, str) and rivers in self.geoms:
+                    gdf_riv = self.geoms[rivers].copy()
+                else:
+                    gdf_riv = self.data_catalog.get_geodataframe(
+                        rivers,
+                        geom=self.mask.raster.box,
+                        buffer=1e3,  # 1km
+                    ).to_crs(self.crs)
+                # update missing attributes based on global values
+                for key in attrs:
+                    if key in dataset:
+                        value = dataset.pop(key)
+                        if key not in gdf_riv.columns:  # update all
+                            gdf_riv[key] = value
+                        elif np.any(np.isnan(gdf_riv[key])):  # fill na
+                            gdf_riv[key] = gdf_riv[key].fillna(value)
+                if not gdf_riv.columns.isin(["rivbed", "rivdph"]).any():
+                    raise ValueError("No 'rivbed' or 'rivdph' attribute found.")
+            else:
+                raise ValueError("No 'centerlines' dataset provided.")
+            dd.update({"gdf_riv": gdf_riv})
+
+            # parse mask
+            if "mask" in dataset:
+                gdf_riv_mask = self.data_catalog.get_geodataframe(
+                    dataset.get("mask"),
+                    geom=self.mask.raster.box,
+                )
+                dd.update({"gdf_riv_mask": gdf_riv_mask})
+            elif "rivwth" not in gdf_riv:
+                raise ValueError(
+                    "Either mask must be provided or centerlines "
+                    "should contain a 'rivwth' attribute."
+                )
+
+            # copy remaining keys
+            for key, value in dataset.items():
+                if key in copy_keys and key not in dd:
+                    dd.update({key: value})
+                elif key not in copy_keys + parse_keys:
+                    self.logger.warning(f"Unknown key {key} in datasets_riv. Ignoring.")
+            datasets_out.append(dd)
+
+        return datasets_out
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/sfincs_input.py` & `hydromt_sfincs-1.0.1/hydromt_sfincs/sfincs_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                 [vals.append(float(val)) for val in val.split()]
                 val = vals
             elif name == "utmzone":
                 val = str(val)
             else:
                 try:
                     val = literal_eval(val)
-                except ValueError:  # normal string
+                except Exception:  # normal string
                     pass
             if name == "crs":
                 name = "epsg"
             inp_dict[name] = val
             setattr(self, name, val)
 
         # set default values to None if not found in inp_dict to avoid writing these later
```

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/subgrid.py` & `hydromt_sfincs-1.0.1/hydromt_sfincs/subgrid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 SubgridTableRegular class to create, read and write sfincs subgrid (sbg) files.
 """
+import gc
+import logging
 import os
 
 import numpy as np
-import logging
 import rasterio
 import xarray as xr
 from numba import njit
 from rasterio.windows import Window
+from scipy import ndimage
 
 from . import workflows
 
 logger = logging.getLogger(__name__)
 
 
 class SubgridTableRegular:
@@ -90,15 +92,15 @@
 
         self.u_zmin[iok[0], iok[1]] = np.fromfile(
             file, dtype=np.float32, count=self.nr_cells
         )
         self.u_zmax[iok[0], iok[1]] = np.fromfile(
             file, dtype=np.float32, count=self.nr_cells
         )
-        dhdz = np.fromfile(file, dtype=np.float32, count=self.nr_cells)  # not used
+        _ = np.fromfile(file, dtype=np.float32, count=self.nr_cells)  # not used
         for ibin in range(self.nbins):
             self.u_hrep[ibin, iok[0], iok[1]] = np.fromfile(
                 file, dtype=np.float32, count=self.nr_cells
             )
         for ibin in range(self.nbins):
             self.u_navg[ibin, iok[0], iok[1]] = np.fromfile(
                 file, dtype=np.float32, count=self.nr_cells
@@ -106,15 +108,15 @@
 
         self.v_zmin[iok[0], iok[1]] = np.fromfile(
             file, dtype=np.float32, count=self.nr_cells
         )
         self.v_zmax[iok[0], iok[1]] = np.fromfile(
             file, dtype=np.float32, count=self.nr_cells
         )
-        dhdz = np.fromfile(file, dtype=np.float32, count=self.nr_cells)  # not used
+        _ = np.fromfile(file, dtype=np.float32, count=self.nr_cells)  # not used
         for ibin in range(self.nbins):
             self.v_hrep[ibin, iok[0], iok[1]] = np.fromfile(
                 file, dtype=np.float32, count=self.nr_cells
             )
         for ibin in range(self.nbins):
             self.v_navg[ibin, iok[0], iok[1]] = np.fromfile(
                 file, dtype=np.float32, count=self.nr_cells
@@ -183,123 +185,137 @@
         file.close()
 
     def build(
         self,
         da_mask: xr.DataArray,
         datasets_dep: list[dict],
         datasets_rgh: list[dict] = [],
+        datasets_riv: list[dict] = [],
         nbins=10,
         nr_subgrid_pixels=20,
         nrmax=2000,
         max_gradient=5.0,
         z_minimum=-99999.0,
         manning_land: float = 0.04,
         manning_sea: float = 0.02,
         rgh_lev_land: float = 0.0,
         buffer_cells: int = 0,
+        extrapolate_values: bool = False,
         write_dep_tif: bool = False,
         write_man_tif: bool = False,
         highres_dir: str = None,
         logger=logger,
     ):
-        """Create subgrid tables for regular grid based on a list of depth and Manning's n datasets.
+        """Create subgrid tables for regular grid based on a list of depth,
+        Manning's rougnhess and river datasets.
 
         Parameters
         ----------
         da_mask : xr.DataArray
-            Mask of the SFINCS domain, with 1,2,3 for active (and boundary) cells and 0 for inactive cells.
+            Mask of the SFINCS domain, with 1,2,3 for active (and boundary) cells
+            and 0 for inactive cells.
         datasets_dep : List[dict]
-            List of dictionaries with topobathy data, each containing an xarray.DataSet and optional merge arguments e.g.:
-            [{'da': merit_hydro_da, 'zmin': 0.01}, {'da': gebco_da, 'offset': 0, 'merge_method': 'first', reproj_method: 'bilinear'}]
-            For a complete overview of all merge options, see :py:function:~hydromt.workflows.merge_multi_dataarrays
+            List of dictionaries with topobathy data, each containing an xarray.DataSet
+            and optional merge arguments e.g.:
+            [
+                {'da': <xr.Dataset>, 'zmin': 0.01},
+                {'da': <xr.Dataset>, 'merge_method': 'first', reproj_method: 'bilinear'}
+            ]
+            For a complete overview of all merge options,
+            see :py:function:~hydromt.workflows.merge_multi_dataarrays
         datsets_rgh : List[dict], optional
-            List of dictionaries with Manning's n data, each containing an xarray.DataSet with manning values and optional merge arguments
+            List of dictionaries with Manning's n data, each containing an
+            xarray.DataSet with manning values and optional merge arguments
+        datasets_riv : List[dict], optional
+            List of dictionaries with river datasets. Each dictionary should at least
+            contain the following:
+            * gdf_riv: line vector of river centerline with
+              river depth ("rivdph") [m] OR bed level ("rivbed") [m+REF],
+              river width ("rivwth"), and
+              river manning ("manning") attributes [m]
+            * gdf_riv_mask (optional): polygon vector of river mask. If provided
+              "rivwth" in river is not used and can be omitted.
+            * arguments for :py:function:~hydromt.workflows.bathymetry.burn_river_rect
+            e.g.: [{'gdf_riv': <gpd.GeoDataFrame>, 'gdf_riv_mask': <gpd.GeoDataFrame>}]
         nbins : int, optional
-            Number of bins in the subgrid tables, by default 10
+            Number of bins in which hypsometry is subdivided, by default 10
         nr_subgrid_pixels : int, optional
             Number of subgrid pixels per computational cell, by default 20
         nrmax : int, optional
             Maximum number of cells per subgrid-block, by default 2000
-            These blocks are used to prevent memory issues while working with large datasets
+            These blocks are used to prevent memory issues
         max_gradient : float, optional
-            Maximum gradient in the subgrid tables, by default 5.0
+            If slope in hypsometry exceeds this value, then smoothing is applied, to
+            prevent numerical stability problems, by default 5.0
         z_minimum : float, optional
             Minimum depth in the subgrid tables, by default -99999.0
         manning_land, manning_sea : float, optional
-            Constant manning roughness values for land and sea, by default 0.04 and 0.02 s.m-1/3
-            Note that these values are only used when no Manning's n datasets are provided, or to fill the nodata values
+            Constant manning roughness values for land and sea,
+            by default 0.04 and 0.02 s.m-1/3
+            Note that these values are only used when no Manning's n datasets are
+            provided, or to fill the nodata values
         rgh_lev_land : float, optional
-            Elevation level to distinguish land and sea roughness (when using manning_land and manning_sea), by default 0.0
+            Elevation level to distinguish land and sea roughness (when using
+            manning_land and manning_sea), by default 0.0
         buffer_cells : int, optional
-            Number of cells between datasets to ensure smooth transition of bed levels, by default 0
+            Number of cells between datasets to ensure smooth transition of bed levels,
+            by default 0
         write_dep_tif : bool, optional
-            Create geotiff of the merged topobathy on the subgrid resolution, by default False
+            Create geotiff of the merged topobathy on the subgrid resolution,
+            by default False
         write_man_tif : bool, optional
-            Create geotiff of the merged roughness on the subgrid resolution, by default False
+            Create geotiff of the merged roughness on the subgrid resolution,
+            by default False
         highres_dir : str, optional
-            Directory where high-resolution geotiffs for topobathy and manning are stored, by default None
+            Directory where high-resolution geotiffs for topobathy and manning
+            are stored, by default None
         """
 
         if write_dep_tif or write_man_tif:
             assert highres_dir is not None, "highres_dir must be specified"
 
         refi = nr_subgrid_pixels
         self.nbins = nbins
         grid_dim = da_mask.raster.shape
         x_dim, y_dim = da_mask.raster.x_dim, da_mask.raster.y_dim
 
-        # determine the output dimensions and transform to match the resolution of da_mask
+        # determine the output dimensions and transform to match da_mask grid
         # NOTE: this is only usef for writing the cloud optimized geotiffs
         output_width = da_mask.sizes[x_dim] * nr_subgrid_pixels
         output_height = da_mask.sizes[y_dim] * nr_subgrid_pixels
         output_transform = da_mask.raster.transform * da_mask.raster.transform.scale(
             1 / nr_subgrid_pixels
         )
 
+        profile = dict(
+            driver="COG",
+            width=output_width,
+            height=output_height,
+            count=1,
+            dtype=np.float32,
+            crs=da_mask.raster.crs,
+            transform=output_transform,
+            blockxsize=256,
+            blockysize=256,
+            compress="deflate",
+            predictor=2,
+            nodata=np.nan,
+            BIGTIFF="YES",  # Add the BIGTIFF option here
+        )
         if write_dep_tif:
             # create the CloudOptimizedGeotiff containing the merged topobathy data
-            dep_tif = rasterio.open(
-                os.path.join(highres_dir, "dep_subgrid.tif"),
-                "w",
-                driver="GTiff",
-                width=output_width,
-                height=output_height,
-                count=1,
-                dtype=np.float32,
-                crs=da_mask.raster.crs,
-                transform=output_transform,
-                tiled=True,
-                blockxsize=256,
-                blockysize=256,
-                compress="deflate",
-                predictor=2,
-                profile="COG",
-                nodata=np.nan,
-            )
+            fn_dep_tif = os.path.join(highres_dir, "dep_subgrid.tif")
+            with rasterio.open(fn_dep_tif, "w", **profile):
+                pass
 
         if write_man_tif:
             # create the CloudOptimizedGeotiff creating the merged manning roughness
-            man_tif = rasterio.open(
-                os.path.join(highres_dir, "manning_subgrid.tif"),
-                "w",
-                driver="GTiff",
-                width=output_width,
-                height=output_height,
-                count=1,
-                dtype=np.float32,
-                crs=da_mask.raster.crs,
-                transform=output_transform,
-                tiled=True,
-                blockxsize=256,
-                blockysize=256,
-                compress="deflate",
-                predictor=2,
-                profile="COG",
-                nodata=np.nan,
-            )
+            fn_man_tif = os.path.join(highres_dir, "manning_subgrid.tif")
+            with rasterio.open(fn_man_tif, "w", **profile):
+                pass
 
         # Z points
         self.z_zmin = np.full(grid_dim, fill_value=np.nan, dtype=np.float32)
         self.z_zmax = np.full(grid_dim, fill_value=np.nan, dtype=np.float32)
         # self.z_zmean = np.full(grid_dim, fill_value=np.nan, dtype=np.float32)
         self.z_volmax = np.full(grid_dim, fill_value=np.nan, dtype=np.float32)
         self.z_depth = np.full((nbins, *grid_dim), fill_value=np.nan, dtype=np.float32)
@@ -354,119 +370,133 @@
                 bn0 = jj * nrcb  # Index of first n in block
                 bn1 = min(bn0 + nrcb, n1)  # last n in block
                 if merge_last_row and jj == (nrbn - 1):
                     bn1 += 1
 
                 # Count
                 ib += 1
-                logger.debug(
-                    f"\nblock {ib + 1}/{nrbn * nrbm} -- "
+                logger.info(
+                    f"block {ib + 1}/{nrbn * nrbm} -- "
                     f"col {bm0}:{bm1-1} | row {bn0}:{bn1-1}"
                 )
 
                 # calculate transform and shape of block at cell and subgrid level
-                da_mask_block = da_mask.isel(
-                    {x_dim: slice(bm0, bm1), y_dim: slice(bn0, bn1)}
-                ).load()
-                assert np.all(
-                    [s > 1 for s in da_mask_block.shape]
-                ), f"unexpected block shape {da_mask_block.shape}"
-                if np.all(da_mask_block == 0):  # not active cells in block
-                    logger.info("Skip block - No active cells")
+                # copy da_mask block to avoid accidently changing da_mask
+                slice_block = {x_dim: slice(bm0, bm1), y_dim: slice(bn0, bn1)}
+                da_mask_block = da_mask.isel(slice_block).load()
+                check_block = np.all([s > 1 for s in da_mask_block.shape])
+                assert check_block, f"unexpected block shape {da_mask_block.shape}"
+                nactive = int(np.sum(da_mask_block > 0))
+                if nactive == 0:  # not active cells in block
+                    logger.debug("Skip block - No active cells")
                     continue
-                logger.info(
-                    f"Processing block with {np.sum(da_mask_block.values):d} active cells .."
-                )
-
+                logger.debug(f"Processing block with {nactive} active cells..")
                 transform = da_mask_block.raster.transform
-                # add refi cells overlap in both dimensions for u and v in last row / col
+                # add refi cells overlap in both dimensions for u and v in last row/col
                 reproj_kwargs = dict(
                     dst_crs=da_mask.raster.crs,
                     dst_transform=transform * transform.scale(1 / refi),
                     dst_width=(da_mask_block.raster.width + 1) * refi,
                     dst_height=(da_mask_block.raster.height + 1) * refi,
                 )
+                da_mask_sbg = da_mask_block.raster.reproject(
+                    method="nearest", **reproj_kwargs
+                ).load()
 
                 # get subgrid bathymetry tile
                 da_dep = workflows.merge_multi_dataarrays(
                     da_list=datasets_dep,
-                    reproj_kwargs=reproj_kwargs,
+                    da_like=da_mask_sbg,
                     interp_method="linear",
                     buffer_cells=buffer_cells,
-                ).load()
+                )
 
                 # set minimum depth
                 da_dep = np.maximum(da_dep, z_minimum)
                 # TODO what to do with remaining cell with nan values
                 # NOTE: this is still open for discussion, but for now we interpolate
-                if np.any(np.isnan(da_dep.values)) > 0:
-                    logger.warning(
-                        f"WARNING: Interpolate data at {int(np.sum(np.isnan(da_dep.values)))} cells"
-                    )
-                    da_dep = da_dep.raster.interpolate_na(method="rio_idw")
-                assert np.all(~np.isnan(da_dep))
+                # raise warning if NaN values in active cells
+                if np.any(np.isnan(da_dep.values[da_mask_sbg > 0])) > 0:
+                    npx = int(np.sum(np.isnan(da_dep.values[da_mask_sbg > 0])))
+                    logger.warning(f"Interpolate data at {npx} subgrid pixels")
+                # always interpolate/extrapolate to avoid NaN values
+                da_dep = da_dep.raster.interpolate_na(
+                    method="rio_idw", extrapolate=True
+                )
 
                 # get subgrid manning roughness tile
                 if len(datasets_rgh) > 0:
                     da_man = workflows.merge_multi_dataarrays(
                         da_list=datasets_rgh,
-                        reproj_kwargs=reproj_kwargs,
+                        da_like=da_mask_sbg,
                         interp_method="linear",
                         buffer_cells=buffer_cells,
-                    ).load()
-                    if np.isnan(da_man).any():
-                        logger.warning("WARNING: nan values in manning roughness array")
-                        da_man0 = xr.where(
-                            da_dep >= rgh_lev_land, manning_land, manning_sea
+                    )
+                    # raise warning if NaN values in active cells
+                    if np.isnan(da_man.values[da_mask_sbg > 0]).any():
+                        logger.debug(
+                            "Missing values in manning roughness array, "
+                            "fill with default values"
                         )
-                        da_man = da_man.where(~np.isnan(da_man), da_man0)
+                    # always fill based on land/sea elevation to avoid NaN values
+                    da_man0 = xr.where(
+                        da_dep >= rgh_lev_land, manning_land, manning_sea
+                    )
+                    da_man = da_man.where(~np.isnan(da_man), da_man0)
                 else:
                     da_man = xr.where(da_dep >= rgh_lev_land, manning_land, manning_sea)
-                assert np.all(~np.isnan(da_man))
+                    da_man.raster.set_nodata(np.nan)
+
+                # burn rivers in bathymetry and manning
+                if len(datasets_riv) > 0:
+                    logger.debug("Burn rivers in bathymetry and manning data")
+                    for riv_kwargs in datasets_riv:
+                        da_dep, da_man = workflows.bathymetry.burn_river_rect(
+                            da_elv=da_dep, da_man=da_man, logger=logger, **riv_kwargs
+                        )
 
                 # optional write tile to file
                 # NOTE tiles have overlap! da_dep[:-refi,:-refi]
+                window = Window(
+                    bm0 * nr_subgrid_pixels,
+                    bn0 * nr_subgrid_pixels,
+                    da_dep[:-refi, :-refi].sizes[x_dim],
+                    da_dep[:-refi, :-refi].sizes[y_dim],
+                )
                 if write_dep_tif:
                     # write the block to the output COG
-                    window = Window(
-                        bm0 * nr_subgrid_pixels,
-                        bn0 * nr_subgrid_pixels,
-                        da_dep[:-refi, :-refi].sizes[x_dim],
-                        da_dep[:-refi, :-refi].sizes[y_dim],
-                    )
-                    dep_tif.write(
-                        da_dep[:-refi, :-refi].values.astype(dep_tif.dtypes[0]),
-                        window=window,
-                        indexes=1,
-                    )
-
+                    with rasterio.open(fn_dep_tif, "r+") as dep_tif:
+                        dep_tif.write(
+                            da_dep.where(da_mask_sbg > 0)[:-refi, :-refi].values,
+                            window=window,
+                            indexes=1,
+                        )
                 if write_man_tif:
-                    # write the block to the output COG
-                    window = Window(
-                        bm0 * nr_subgrid_pixels,
-                        bn0 * nr_subgrid_pixels,
-                        da_man[:-refi, :-refi].sizes[x_dim],
-                        da_man[:-refi, :-refi].sizes[y_dim],
-                    )
-                    man_tif.write(
-                        da_man[:-refi, :-refi].values.astype(man_tif.dtypes[0]),
-                        window=window,
-                        indexes=1,
-                    )
+                    with rasterio.open(fn_man_tif, "r+") as man_tif:
+                        man_tif.write(
+                            da_man.where(da_mask_sbg > 0)[:-refi, :-refi].values,
+                            window=window,
+                            indexes=1,
+                        )
+
+                # check for NaN values for entire tile
+                check_nans = np.all(np.isfinite(da_dep))
+                assert check_nans, "NaN values in depth array"
+                check_nans = np.all(np.isfinite(da_man))
+                assert check_nans, "NaN values in manning roughness array"
 
                 yg = da_dep.raster.ycoords.values
                 if yg.ndim == 1:
                     yg = np.repeat(np.atleast_2d(yg), da_dep.raster.shape[0], axis=0)
 
                 # Now compute subgrid properties
                 sn, sm = slice(bn0, bn1), slice(bm0, bm1)
                 (
                     self.z_zmin[sn, sm],
                     self.z_zmax[sn, sm],
-                    # self.z_zmean[sn, sm],
                     self.z_volmax[sn, sm],
                     self.z_depth[:, sn, sm],
                     self.u_zmin[sn, sm],
                     self.u_zmax[sn, sm],
                     self.u_hrep[:, sn, sm],
                     self.u_navg[:, sn, sm],
                     self.v_zmin[sn, sm],
@@ -483,21 +513,17 @@
                     nbins,
                     yg,
                     max_gradient,
                     da_mask.raster.crs.is_geographic,
                 )
 
                 del da_mask_block, da_dep, da_man
+                gc.collect()
 
-        # close the output cloud optimized geotiff
-        if write_dep_tif:
-            dep_tif.close()
-
-        if write_man_tif:
-            man_tif.close()
+        # TODO build COG overviews
 
     def to_xarray(self, dims, coords):
         """Convert subgrid class to xarray dataset."""
         ds_sbg = xr.Dataset(coords={"bins": np.arange(self.nbins), **coords})
         ds_sbg.attrs.update({"_FillValue": np.nan})
 
         zlst2 = ["z_zmin", "z_zmax", "z_zmin", "z_volmax"]  # "z_zmean",
@@ -541,16 +567,16 @@
     # V points
     v_zmin = np.full(grid_dim, fill_value=np.nan, dtype=np.float32)
     v_zmax = np.full(grid_dim, fill_value=np.nan, dtype=np.float32)
     v_hrep = np.full((nbins, *grid_dim), fill_value=np.nan, dtype=np.float32)
     v_navg = np.full((nbins, *grid_dim), fill_value=np.nan, dtype=np.float32)
 
     # Loop through all active cells in this block
-    for n in range(mask.shape[0]):
-        for m in range(mask.shape[1]):
+    for n in range(mask.shape[0]):  # row
+        for m in range(mask.shape[1]):  # col
             if mask[n, m] < 1:
                 # Not an active point
                 continue
 
             nn = int(n * refi)
             mm = int(m * refi)
 
@@ -561,49 +587,47 @@
                 dypm = float(dyp * 111111.0)
             else:
                 dxpm = float(dxp)
                 dypm = float(dyp)
 
             # First the volumes in the cells
             zgc = zg[nn : nn + refi, mm : mm + refi]
-            zv = zgc.flatten()
             zvmin = -20.0
-            z, v, zmin, zmax, zmean = subgrid_v_table(
-                zv, dxpm, dypm, nbins, zvmin, max_gradient
+            z, v, zmin, zmax = subgrid_v_table(
+                zgc.flatten(), dxpm, dypm, nbins, zvmin, max_gradient
             )
             z_zmin[n, m] = zmin
             z_zmax[n, m] = zmax
-            # z_zmean[n, m] = zmean
             z_volmax[n, m] = v[-1]
             z_depth[:, n, m] = z[1:]
 
             # Now the U/V points
             # U
             nn = n * refi
             mm = m * refi + int(0.5 * refi)
             zgu = zg[nn : nn + refi, mm : mm + refi]
             zgu = np.transpose(zgu)
-            zv = zgu.flatten()
             manning = manning_grid[nn : nn + refi, mm : mm + refi]
             manning = np.transpose(manning)
-            manning = manning.flatten()
-            zmin, zmax, hrep, navg, zz = subgrid_q_table(zv, manning, nbins)
+            zmin, zmax, hrep, navg, zz = subgrid_q_table(
+                zgu.flatten(), manning.flatten(), nbins
+            )
             u_zmin[n, m] = zmin
             u_zmax[n, m] = zmax
             u_hrep[:, n, m] = hrep
             u_navg[:, n, m] = navg
 
             # V
             nn = n * refi + int(0.5 * refi)
             mm = m * refi
             zgu = zg[nn : nn + refi, mm : mm + refi]
-            zv = zgu.flatten()
             manning = manning_grid[nn : nn + refi, mm : mm + refi]
-            manning = manning.flatten()
-            zmin, zmax, hrep, navg, zz = subgrid_q_table(zv, manning, nbins)
+            zmin, zmax, hrep, navg, zz = subgrid_q_table(
+                zgu.flatten(), manning.flatten(), nbins
+            )
             v_zmin[n, m] = zmin
             v_zmax[n, m] = zmax
             v_hrep[:, n, m] = hrep
             v_navg[:, n, m] = navg
 
     return (
         z_zmin,
@@ -633,31 +657,47 @@
 
 @njit
 def isclose(a, b, rtol=1e-05, atol=1e-08):
     return abs(a - b) <= (atol + rtol * abs(b))
 
 
 @njit
-def subgrid_v_table(elevation, dx, dy, nbins, zvolmin, max_gradient):
+def subgrid_v_table(
+    elevation: np.ndarray,
+    dx: float,
+    dy: float,
+    nbins: int,
+    zvolmin: float,
+    max_gradient: float,
+):
     """
-    map vector of elevation values into a hypsometric volume - depth relationship for one grid cell
+    map vector of elevation values into a hypsometric volume - depth relationship
+    for one grid cell
 
     Parameters
     ----------
-    elevation : np.ndarray (nr of pixels in one cell) containing subgrid elevation values for one grid cell [m]
-    dx: float, x-directional cell size (typically not known at this level) [m]
-    dy: float, y-directional cell size (typically not known at this level) [m]
-    nbins: int, number of bins to use for the hypsometric curve
-    zvolmin: float, minimum elevation value to use for volume calculation (typically -20 m)
-    max_gradient: float, maximum gradient to use for volume calculation (typically 0.1)
+    elevation: np.ndarray
+        subgrid elevation values for one grid cell [m]
+    dx: float
+        x-directional cell size (typically not known at this level) [m]
+    dy: float
+        y-directional cell size (typically not known at this level) [m]
+    nbins: int
+        number of bins to use for the hypsometric curve
+    zvolmin: float
+        minimum elevation value to use for volume calculation (typically -20 m)
+    max_gradient: float
+        maximum gradient to use for volume calculation (typically 0.1)
 
     Return
     ------
-    ele_sort : np.ndarray (1D flattened from elevation) with sorted and flattened elevation values
-    volume : np.ndarray (1D flattened from elevation) containing volumes (lowest value zero) per sorted elevation value
+    z, V: np.ndarray
+        sorted elevation values, volume per elevation value
+    zmin, zmax: float
+        minimum, and maximum elevation values
     """
 
     # Cell area
     a = float(elevation.size * dx * dy)
 
     # Set minimum elevation to -20 (needed with single precision), and sort
     ele_sort = np.sort(np.maximum(elevation, zvolmin).flatten())
@@ -685,35 +725,39 @@
         dzdh.max() > max_gradient and not (isclose(dzdh.max(), max_gradient))
     ) and n < nbins:
         # reshape until gradient is satisfactory
         idx = np.where(dzdh == dzdh.max())[0]
         z[idx + 1] = z[idx] + max_gradient * (dvol / a)
         dzdh = get_dzdh(z, V, a)
         n += 1
-    return z, V, elevation.min(), z.max(), ele_sort.mean()
+    return z, V, elevation.min(), z.max()
 
 
 @njit
-def subgrid_q_table(elevation, manning, nbins):
+def subgrid_q_table(elevation: np.ndarray, manning: np.ndarray, nbins: int):
     """
-    map vector of elevation values into a hypsometric hydraulic radius - depth relationship for one grid cell
+    map elevation values into a hypsometric hydraulic radius - depth relationship
 
     Parameters
     ----------
-    elevation : np.ndarray (nr of pixels in one cell) containing subgrid elevation values for one grid cell [m]
-    manning : np.ndarray (nr of pixels in one cell) containing subgrid manning roughness values for one grid cell [s m^(-1/3)]
-    nbins : int, number of bins to use for the hypsometric curve
-    dx : float, x-directional cell size (typically not known at this level) [m]
-    dy : float, y-directional cell size (typically not known at this level) [m]
+    elevation: np.ndarray
+        subgrid elevation values for one grid cell [m]
+    manning: np.ndarray
+        subgrid manning roughness values for one grid cell [s m^(-1/3)]
+    nbins: int
+        number of bins to use for the hypsometric curve
 
     Returns
     -------
-    ele_sort, R : np.ndarray of sorted elevation values, np.ndarray of sorted hydraulic radii that belong with depth
+    zmin, zmax: float
+        minimum and maximum elevation values used for hypsometric curve
+    hrep, navg, zz: np.ndarray
+        conveyance depth, average manning roughness, and elevation values
+        for each bin
     """
-
     hrep = np.zeros(nbins, dtype=np.float32)
     navg = np.zeros(nbins, dtype=np.float32)
     zz = np.zeros(nbins, dtype=np.float32)
 
     n = int(elevation.size)  # Nr of pixels in grid cell
     n05 = int(n / 2)
 
@@ -741,13 +785,11 @@
 
         ibelow = np.where(elevation <= zbin)  # index of pixels below bin level
         # water depth in each pixel
         h = np.maximum(zbin - np.maximum(elevation, zmin), 0.0)
         qi = h ** (5.0 / 3.0) / manning  # unit discharge in each pixel
         q = np.sum(qi) / n  # combined unit discharge for cell
 
-        if not np.any(manning[ibelow]):
-            print("NaNs found?!")
         navg[ibin] = manning[ibelow].mean()  # mean manning's n
         hrep[ibin] = (q * navg[ibin]) ** (3.0 / 5.0)  # conveyance depth
 
     return zmin, zmax, hrep, navg, zz
```

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/utils.py` & `hydromt_sfincs-1.0.1/hydromt_sfincs/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     "mask2gdf",
     "read_xy",
     "write_xy",
     "read_xyn",
     "write_xyn",
     "read_geoms",
     "write_geoms",
+    "read_drn",
+    "write_drn",
     "gdf2linestring",
     "gdf2polygon",
     "linestring2gdf",
     "polygon2gdf",
     "read_sfincs_map_results",
     "read_sfincs_his_results",
     "downscale_floodmap",
@@ -235,17 +237,17 @@
         for point in gdf.iterfeatures():
             x, y = point["geometry"]["coordinates"]
             try:
                 name = point["properties"]["name"]
             except:
                 name = "obs" + str(point["id"])
             if crs.is_geographic:
-                string = f'{x:12.6f}{y:12.6f}  "{name}"\n'
+                string = f"{x:12.6f}{y:12.6f}  {name}\n"
             else:
-                string = f'{x:12.1f}{y:12.1f}  "{name}"\n'
+                string = f"{x:12.1f}{y:12.1f}  {name}\n"
             fid.write(string)
 
 
 ## ASCII TIMESERIES: bzs / dis / precip ##
 
 
 def parse_datetime(dt: Union[str, datetime], format="%Y%m%d %H%M%S") -> datetime:
@@ -311,15 +313,15 @@
     tref = parse_datetime(tref)
     if df.index.size == 0:
         raise ValueError("df does not contain data.")
     data = df.reset_index().values
     data[:, 0] = (df.index - tref).total_seconds()
     # calculate required width for time column; hard coded single decimal precision
     # format for other columns is based on fmt`argument
-    w = int(np.floor(np.log10(data[-1, 0]))) + 3
+    w = int(np.floor(np.log10(abs(data[-1, 0])))) + 3
     fmt_lst = [f"%{w}.1f"] + [fmt for _ in range(df.columns.size)]
     fmt_out = " ".join(fmt_lst)
     with open(fn, "w") as f:
         np.savetxt(f, data, fmt=fmt_out)
 
 
 ## MASK
@@ -418,17 +420,17 @@
         List of dictionaries describing structures.
     """
     feats = []
     for _, item in gdf.iterrows():
         feat = item.drop("geometry").dropna().to_dict()
         # check geom
         line = item.geometry
-        if line.type == "MultiLineString" and len(line.geoms) == 1:
+        if line.geom_type == "MultiLineString" and len(line.geoms) == 1:
             line = line.geoms[0]
-        if line.type != "LineString":
+        if line.geom_type != "LineString":
             raise ValueError("Invalid geometry type, only LineString is accepted.")
         xyz = tuple(zip(*line.coords[:]))
         feat["x"], feat["y"] = list(xyz[0]), list(xyz[1])
         if len(xyz) == 3:
             feat["z"] = list(xyz[2])
         feats.append(feat)
     return feats
@@ -534,18 +536,19 @@
 
     Parameters
     ----------
     fn: str, Path
         Path to output structure file.
     feats: list of dict
         List of dictionaries describing structures.
-        For pli, pol and thd files "x" and "y" are required, "name" is optional.
+        For pli, pol, thd anc crs files "x" and "y" are required, "name" is optional.
         For weir files "x", "y" and "z" are required, "name" and "par1" are optional.
-    stype: {'pli', 'pol', 'thd', 'weir'}
-        Geom type polylines (pli), polygons (pol) thin dams (thd) or weirs (weir).
+    stype: {'pli', 'pol', 'thd', 'weir', 'crs'}
+        Geom type polylines (pli), polygons (pol) thin dams (thd), weirs (weir)
+        or cross-sections (crs).
     fmt: str
         format for "z" and "par1" fields.
 
     Examples
     --------
     >>> feats = [
             {
@@ -561,15 +564,15 @@
                 "y": [100, 100, 100],
                 "z": [5.0, 5.1, 5.0],
                 "par1": 0.6,
             },
         ]
     >>> write_structures('sfincs.weir', feats, stype='weir')
     """
-    cols = {"pli": 2, "pol": 2, "thd": 2, "weir": 4}[stype.lower()]
+    cols = {"pli": 2, "pol": 2, "thd": 2, "weir": 4, "crs": 2}[stype.lower()]
     fmt = ["%.0f", "%.0f"] + [fmt for _ in range(cols - 2)]
     if stype.lower() == "weir" and np.any(["z" not in f for f in feats]):
         raise ValueError('"z" value missing for weir files.')
     with open(fn, "w") as f:
         for i, feat in enumerate(feats):
             name = feat.get("name", i + 1)
             if isinstance(name, int):
@@ -619,14 +622,106 @@
                 for c in col_names[2:]:
                     if np.unique(feat[c]).size == 1:
                         feat[c] = feat[c][0]
             feats.append(feat)
     return feats
 
 
+def write_drn(fn: Union[str, Path], gdf_drainage: gpd.GeoDataFrame, fmt="%.4f") -> None:
+    """Write structure files from list of dictionaries.
+
+    Parameters
+    ----------
+    fn : str, Path
+        Path to structure file.
+    drainage : gpd.GeoDataFrame
+        Dataframe with drainage structure parameters and geometry.
+    fmt : str
+        Format for float values.
+    """
+
+    # expected columns for drainage structures
+    col_names = [
+        "xsnk",
+        "ysnk",
+        "xsrc",
+        "ysrc",
+        "type",
+        "par1",
+        "par2",
+        "par3",
+        "par4",
+        "par5",
+    ]
+
+    gdf = copy.deepcopy(gdf_drainage)
+    # get geometry linestring and convert to xsnk, ysnk, xsrc, ysrc
+    endpoints = gdf.boundary.explode().unstack()
+    gdf["xsnk"] = endpoints[0].x
+    gdf["ysnk"] = endpoints[0].y
+    gdf["xsrc"] = endpoints[1].x
+    gdf["ysrc"] = endpoints[1].y
+    gdf.drop(["geometry"], axis=1, inplace=True)
+
+    # reorder columns based on col_names
+    gdf = gdf[col_names]
+
+    # write to file
+    gdf.to_csv(fn, sep=" ", index=False, header=False, float_format=fmt)
+
+
+def read_drn(fn: Union[str, Path], crs: int = None) -> gpd.GeoDataFrame:
+    """Read drainage structure files to geodataframe.
+
+    Parameters
+    ----------
+    fn : str, Path
+        Path to drainge structure file.
+    crs : int
+        EPSG code for coordinate reference system.
+
+    Returns
+    -------
+    gpd.GeoDataFrame
+        Dataframe with drainage structure parameters and geometry.
+    """
+
+    # expected columns for drainage structures
+    col_names = [
+        "xsnk",
+        "ysnk",
+        "xsrc",
+        "ysrc",
+        "type",
+        "par1",
+        "par2",
+        "par3",
+        "par4",
+        "par5",
+    ]
+
+    # read structure file
+    df = pd.read_csv(fn, sep="\\s+", names=col_names)
+
+    # get geometry linestring
+    geom = [
+        LineString([(xsnk, ysnk), (xsrc, ysrc)])
+        for xsnk, ysnk, xsrc, ysrc in zip(
+            df["xsnk"], df["ysnk"], df["xsrc"], df["ysrc"]
+        )
+    ]
+    df.drop(["xsnk", "ysnk", "xsrc", "ysrc"], axis=1, inplace=True)
+
+    # convert to geodataframe
+    gdf = gpd.GeoDataFrame(df, geometry=geom)
+    if crs is not None:
+        gdf.set_crs(crs, inplace=True)
+    return gdf
+
+
 ## OUTPUT: sfincs_map.nc, sfincs_his.nc ##
 
 
 def read_sfincs_map_results(
     fn_map: Union[str, Path],
     ds_like: xr.Dataset,
     chunksize: int = 100,
@@ -667,14 +762,18 @@
     ds_map = ds_map.rename(
         {k: v for k, v in rm.items() if (k in ds_map or k in ds_map.dims)}
     )
     ds_map = ds_map.set_coords(
         [var for var in ds_map.data_vars.keys() if (var in rm.values())]
     )
 
+    # support for older sfincs_map.nc files
+    # check if x,y dimensions are in the order y,x
+    ds_map = ds_map.transpose(..., "y", "x", "corner_y", "corner_x")
+
     # split face and edge variables
     scoords = ds_like.raster.coords
     tcoords = {tdim: ds_map[tdim] for tdim in ds_map.dims if tdim.startswith("time")}
     ds_face = xr.Dataset(coords={**scoords, **tcoords})
     ds_edge = xr.Dataset()
     for var in ds_map.data_vars:
         if var in drop:
@@ -715,15 +814,15 @@
     Returns
     -------
     ds_his: xr.Dataset
         Parsed SFINCS output his file.
     """
 
     ds_his = xr.open_dataset(fn_his, chunks={"time": chunksize}, **kwargs)
-    crs = ds_his["crs"].item() if ds_his["crs"].item() != 0 else crs
+    crs = ds_his["crs"].item() if ds_his["crs"].item() > 0 else crs
     dvars = list(ds_his.data_vars.keys())
     # set coordinates & spatial dims
     cvars = ["id", "name", "x", "y"]
     ds_his = ds_his.set_coords([v for v in dvars if v.split("_")[-1] in cvars])
     ds_his.vector.set_spatial_dims(
         x_name="station_x", y_name="station_y", index_dim="stations"
     )
```

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/discharge.py` & `hydromt_sfincs-1.0.1/hydromt_sfincs/workflows/discharge.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,39 +50,39 @@
     ds_wdw = ds.raster.sample(gdf, wdw=wdw)
     # check if valid discharge
     valid = ds_wdw[discharge_name].notnull().any("time")
     if uparea_name in ds and uparea_name in gdf.columns:
         logger.debug(
             f"Snapping {discharge_name} points to best matching uparea cell within wdw (size={wdw})."
         )
+        # find cells in window with smallest difference in uparea
         upa0 = xr.DataArray(gdf[uparea_name], dims=("index"))
         upa_dff = np.abs(
             ds_wdw[uparea_name].where(ds_wdw[uparea_name] > 0).load() - upa0
         )
+        i_wdw = upa_dff.fillna(np.inf).argmin("wdw")
+        # find valid cells based on error criteria
         upa_check = np.logical_or((upa_dff / upa0) <= rel_error, upa_dff <= abs_error)
         valid = np.logical_and(valid, upa_check)
-        # combine valid local cells with best matching windows cells if local cell invalid
-        # i_loc = int((1 + 2 * wdw) ** 2 / 2)  # center cell
-        # i_wdw = upa_dff.argmin("wdw").where(~valid.isel(wdw=i_loc), i_loc).load()
-        # find best matching uparea cell in window
-        i_wdw = upa_dff.argmin("wdw").load()
     else:
         logger.debug(
             f"No {uparea_name} variable found in ds or gdf; "
             f"sampling {discharge_name} points from nearest grid cell."
         )
-        # add distance (measured in cells)
+        # calculate distance to center cell (measured in cells)
         ar_wdw = np.abs(np.arange(-wdw, wdw + 1))
         dist = np.hypot(**np.meshgrid(ar_wdw, ar_wdw)).ravel()
         ds_wdw["dist"] = xr.Variable(
             ("index", "wdw"), np.tile(dist, (ds_wdw["index"].size, 1))
         )
+        # find nearest valid cell in window
         i_wdw = ds_wdw["dist"].where(valid, np.inf).argmin("wdw").load()
+    # filter valid cells
     idx_valid = np.where(valid.isel(wdw=i_wdw).values)[0]
     if idx_valid.size < gdf.index.size:
         logger.warning(
             f"{idx_valid.size}/{gdf.index.size} {discharge_name} points successfully snapped."
         )
     i_wdw = i_wdw.isel(index=idx_valid)
+    # return discharge at valid cells
     ds_out = ds_wdw.isel(wdw=i_wdw.load(), index=idx_valid)
-
-    return ds_out  # .reset_coords()[discharge_name]
+    return ds_out
```

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/flwdir.py` & `hydromt_sfincs-1.0.1/hydromt_sfincs/workflows/flwdir.py`

 * *Files identical despite different names*

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/landuse.py` & `hydromt_sfincs-1.0.1/hydromt_sfincs/workflows/landuse.py`

 * *Files identical despite different names*

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/merge.py` & `hydromt_sfincs-1.0.1/hydromt_sfincs/workflows/merge.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 from typing import Dict, List, Union
 
 import geopandas as gpd
 import numpy as np
 import xarray as xr
 from scipy import ndimage
 
+from .bathymetry import burn_river_rect
+
 logger = logging.getLogger(__name__)
 
 __all__ = ["merge_multi_dataarrays", "merge_dataarrays"]
 
 
 def merge_multi_dataarrays(
     da_list: List[dict],
+    gdf_list: List[dict] = [],
     da_like: xr.DataArray = None,
     reproj_kwargs: Dict = {},
     buffer_cells: int = 0,  # not in list
     interp_method: str = "linear",  # not in list
     logger=logger,
 ) -> xr.DataArray:
     """Merge a list of data arrays by reprojecting these to a common destination grid
@@ -84,16 +87,26 @@
             method = "bilinear"
         else:
             method = "average"
     else:
         method = "bilinear"
 
     if da_like is not None:  # reproject first raster to destination grid
-        da1 = da1.raster.reproject_like(da_like, method=method).load()
+        # clip before reproject
+        bbox = da_like.raster.transform_bounds(da1.raster.crs)
+        da1 = da1.raster.clip_bbox(bbox, buffer=2)
+        if np.any(np.array(da1.shape) <= 2):
+            # no data in da1 so use an empty array like da_like
+            logger.debug("No data da1, start with empty array")
+            da1 = xr.full_like(da_like, np.nan)
+        else:
+            # TODO: this applies to the whole dataset, not only the clipped part
+            da1 = da1.load().raster.reproject_like(da_like)
     elif reproj_kwargs:
+        # TODO
         da1 = da1.raster.reproject(method=method, **reproj_kwargs).load()
     logger.debug(f"Reprojection method of first dataset is: {method}")
 
     # set nodata to np.nan, Note this might change the dtype to float
     da1 = da1.raster.mask_nodata()
 
     # get valid cells of first dataset
@@ -111,14 +124,15 @@
         merge_method = da_list[i].get("merge_method", "first")
         if merge_method == "first" and not np.any(np.isnan(da1.values)):
             continue
 
         # base reprojection method on resolution of datasets
         reproj_method = da_list[i].get("reproj_method", None)
         da2 = da_list[i].get("da")
+
         if reproj_method is None:
             dx_2 = (
                 np.abs(da2.raster.res[0])
                 if not da2.raster.crs.is_geographic
                 else np.abs(da2.raster.res[0]) * 111111.0
             )
             if dx_2 >= dx_1:
@@ -138,14 +152,30 @@
             gdf_valid=da_list[i].get("gdf_valid", None),
             reproj_method=reproj_method,
             merge_method=merge_method,
             buffer_cells=buffer_cells,
             interp_method=interp_method,
         )
 
+    # burn in rivers
+    for i in range(len(gdf_list)):
+        cs_type = gdf_list[i].get("type", "rectangular")
+        if cs_type == "rectangular":
+            # width or gdf_riv_mask is required
+            # zb is used if provided, otherwise depth is used
+            da1 = burn_river_rect(
+                da_elv=da1,
+                gdf_riv=gdf_list[i].get("gdf"),
+                gdf_riv_mask=gdf_list[i].get("gdf_mask", None),
+                rivdph_name=gdf_list[i].get("depth", "rivdph"),
+                rivwth_name=gdf_list[i].get("width", "rivwth"),
+                rivbed_name=gdf_list[i].get("zb", "rivbed"),
+            )
+        else:
+            raise NotImplementedError(f"Cross section type {cs_type} not implemented.")
     return da1
 
 
 def merge_dataarrays(
     da1: xr.DataArray,
     da2: xr.DataArray,
     offset: Union[xr.DataArray, float] = None,
@@ -203,23 +233,24 @@
         Merged dataarray
     """
 
     nodata = da1.raster.nodata
     dtype = da1.dtype
     if not np.isnan(nodata):
         da1 = da1.raster.mask_nodata()
+    # clip before reproject
+    bbox = da1.raster.transform_bounds(da2.raster.crs)
+    da2 = da2.raster.clip_bbox(bbox, buffer=2)
+    if np.any(np.array(da2.shape) <= 2):
+        logger.debug(f"No data in dataset 2 within bbox [{bbox}], skip")
+        return da1
+
     ## reproject da2 and reset nodata value to match da1 nodata
-    try:
-        da2 = (
-            da2.raster.reproject_like(da1, method=reproj_method)
-            .raster.mask_nodata()
-            .load()
-        )
-    except:
-        print("No data for this tile")
+    da2 = da2.load().raster.reproject_like(da1, method=reproj_method)
+    da2 = da2.raster.mask_nodata()
 
     da2 = _add_offset_mask_invalid(
         da=da2,
         offset=offset,
         min_valid=min_valid,
         max_valid=max_valid,
         gdf_valid=gdf_valid,
@@ -252,14 +283,15 @@
         da_out = da_out.where(~mask_buf, da_out_interp)
 
     da_out = da_out.fillna(nodata).astype(dtype)
     da_out.raster.set_nodata(nodata)
     return da_out
 
 
+## Helper functions
 def _add_offset_mask_invalid(
     da,
     offset=None,
     min_valid=None,
     max_valid=None,
     gdf_valid=None,
     reproj_method: str = "bilinear",
```

### Comparing `hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/tiling.py` & `hydromt_sfincs-1.0.1/hydromt_sfincs/workflows/tiling.py`

 * *Files identical despite different names*

### Comparing `hydromt_sfincs-1.0.0/pyproject.toml` & `hydromt_sfincs-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     {name = "Maarten van Ormondt", email = "Maarten.vanOrmondt@deltares-usa.us"},
     {name = "Dirk Eilander", email = "dirk.eilander@deltares.nl"},
     {name = "Tim Leijnse", email = "tim.leijnse@deltares.nl"},
 ]
 dependencies = [
     "affine",
     "geopandas>=0.8",
-    "hydromt>=0.7.1",
+    "hydromt>=0.8.0,<0.9",
     "numba",
     "numpy",
     "pandas",
     "pillow",
     "pyflwdir>=0.5.5",
     "pyproj",
     "rasterio",
```

### Comparing `hydromt_sfincs-1.0.0/PKG-INFO` & `hydromt_sfincs-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: hydromt_sfincs
-Version: 1.0.0
+Version: 1.0.1
 Summary: hydroMT plugin for sfincs models.
 Author-email: Roel de Goede <roel.degoede@deltares.nl>, Maarten van Ormondt <Maarten.vanOrmondt@deltares-usa.us>, Dirk Eilander <dirk.eilander@deltares.nl>, Tim Leijnse <tim.leijnse@deltares.nl>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: affine
 Requires-Dist: geopandas>=0.8
-Requires-Dist: hydromt>=0.7.1
+Requires-Dist: hydromt>=0.8.0,<0.9
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pillow
 Requires-Dist: pyflwdir>=0.5.5
 Requires-Dist: pyproj
 Requires-Dist: rasterio
@@ -75,17 +75,17 @@
 HydroMT-SFINCS aims to make the model building process **fast**, **modular** and **reproducible**
 and to facilitate the analysis of SFINCS model results
 
 How to use HydroMT-SFINCS?
 --------------------------
 The HydroMT-SFINCS plugin can be used as a **command line + configuration file** application, which provides commands to *build*,
 *update* the SFINCS model with a single line, or **from python** to exploit its rich interface.
-You can learn more about how to use HydroMT-SFINCS in its `online documentation. <docs_getting_started>`_
+You can learn more about how to use HydroMT-SFINCS in its `online documentation. <https://deltares.github.io/hydromt_sfincs/latest/getting_started/intro>`_
 For a smooth installing experience we recommend installing HydroMT-SFINCS and its dependencies
-from conda-forge in a clean environment, see `installation guide. <docs_install>`_
+from conda-forge in a clean environment, see `installation guide. <https://deltares.github.io/hydromt_sfincs/latest/getting_started/installation>`_
 
 How to cite?
 ------------
 To reference the software please use the the DOI provided in the Zenodo badge that points to the latest release |doi|.
 
 The following paper presents a real-world application of HydroMT-SFINCS:
 
@@ -98,16 +98,14 @@
 You can find information about how to contribute to the HydroMT project at our `contributing page. <https://deltares.github.io/hydromt/latest/dev/contributing>`_
 
 HydroMT seeks active contribution from the (hydro) geoscientific community.
 So far, it has been developed and tested with a range of `Deltares <https://www.deltares.nl/en/>`_ models, but
 we believe it is applicable to a much wider set of geoscientific models and are
 happy to discuss how it can be implemented for your model.
 
-.. _docs_getting_started: https://deltares.github.io/hydromt_sfincs/latest/getting_started/intro
-.. _docs_install: https://deltares.github.io/hydromt_sfincs/latest/getting_started/installation
 .. _Hydromt: https://deltares.github.io/hydromt/latest/
 .. _SFINCS: https://sfincs.readthedocs.io/en/latest/
 
 .. |codecov| image:: https://codecov.io/gh/Deltares/hydromt_sfincs/branch/main/graph/badge.svg?token=ss3EgmwHhH
     :target: https://codecov.io/gh/Deltares/hydromt_sfincs
 
 .. |docs_latest| image:: https://img.shields.io/badge/docs-latest-brightgreen.svg
```

