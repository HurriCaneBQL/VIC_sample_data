# WalnutGulch Sample Dataset

### Image Driver

- `image/WalnutGulch/parameters/` - parameter files
    - Global Parameter Files:
        - `WalnutGulch_image_test.global.txt`
            - Domain File: `domain.stehekin.20151028.nc`
            - Parameter File: `WalnutGulch_test_params_20160327.nc`
            - Forcings: `WalnutGulch_image_test.forcings_10days.1949.nc`
        - `global_param.L2015.txt`
            - Domain File: `domain.stehekin.0.0625_deg.nc`
            - Parameter File: `params.WalnutGulch.L2015.nc`
            - Forcings: `WalnutGulch_image_test.forcings_10days.0.0625_deg.1949.nc`
        - `global_param.MOD_IGBP.txt`
            - Domain File: `domain.stehekin.0.0625_deg.nc`
            - Parameter File: `params.WalnutGulch.MOD_IGBP.nc`
            - Forcings: `WalnutGulch_image_test.forcings_10days.0.0625_deg.1949.nc`
            - fcanopy is ignored 
        - `global_param.MOD_IGBP.Fcanopy.txt`
            - Domain File: `domain.stehekin.0.0625_deg.nc`
            - Parameter File: `params.WalnutGulch.MOD_IGBP.nc`
            - Forcings: `WalnutGulch_image_test.forcings_10days.0.0625_deg.1949.nc`
            - fcanopy is used 
    - Domain Files:
        - `domain.stehekin.20151028.nc`
            - 0.125 degree resolution
        - `domain.stehekin.0.0625_deg.nc`
            - 0.0625 degree resolution
            - Taken from Bohn et al. (2018)
    - Parameter Files:
        - `WalnutGulch_test_params_20160327.nc`
            - 0.125 degree resolution
            - NLDAS soil, snow, and veg parameters
        - `WalnutGulch_test_params_20160327.FROZEN_SOIL.nc`
            - Same as `WalnutGulch_test_params_20160327.nc` but has `fs_active=1` in order to run option `FROZEN_SOIL=TRUE`
        - `params.WalnutGulch.L2015.nc`
            - 0.0625 degree resolution
            - Parameters taken from Livneh et al. (2015)
            - NLDAS soil, snow, and veg parameters
        - `params.WalnutGulch.MOD_IGBP.nc`
            - 0.0625 degree resolution
            - MOD-LSP MOD_IGBP parameters (Bohn and Vivoni, 2019)
            - Soils and snowbands from NLDAS
            - Land cover, LAI, fcanopy, and albedo from MODIS
    - RVIC Parameters:
        - `stehekin_parameters_01.rvic.prm.WalnutGulch.20150727.nc`

- `image/WalnutGulch/forcings/` - meteorological forcing files
    - `WalnutGulch_image_test.forcings_10days.1949.nc`
        - 0.125 degree resolution
        - 1-hour time step
        - 10 days of records
    - `WalnutGulch_image_test.forcings_10days.0.0625_deg.1949.nc`
        - 0.0625 degree resolution
        - 1-hour time step
        - 10 days of records

### Classic Driver

Currently there are no classic driver inputs for this dataset.

## References
 - Bohn, T. J, and E. R. Vivoni, 2019: MOD-LSP: MODIS-Based Parameters for Variable Infiltration Capacity (VIC) Model over the Continental US, Mexico, and Southern Canada (Version 1.0) [Data set]. Zenodo, doi:10.5281/zenodo.2612560. https://zenodo.org/record/2612560.
 - Bohn, T. J., K. M. Whitney, G. Mascaro, and E. R. Vivoni, 2018: Parameters for PITRI Precipitation Temporal Disaggregation over continental US, Mexico, and southern Canada, 1981-2013 (Version 1.1) [Data set]. Zenodo, doi:10.5281/zenodo.2564019. http://zenodo.org/record/2564019.
 - Livneh, B., T. J. Bohn, D. W. Pierce, F. Munoz-Arriola, B. Nijssen, R. Vose, D. R. Cayan, and L. Brekke, 2015: A spatially comprehensive, hydrometeorological data set for Mexico, the U.S., and southern Canada 1950–2013. Nat. Sci. Data, 2, 150042, doi:10.1038/sdata.2015.42.