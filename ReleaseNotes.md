ORFLIB Release Notes
====================

VERSION 0.2.0
-------------

### Additions

1. New folder `orflib/math/stats` to contain statistics related source files.

2. New files `orflib/math/stats/errorfunction.hpp` and `errorfunction.cpp`.  
	Definition of class ErrorFunction.

3. New files `orflib/math/stats/univariatedistribution.hpp` and `normaldistribution.hpp`.  
	Definition of `UnivariateDistribution` and `NormalDistribution` classes .

4. New folder `orflib/math/pricers` to contain pricing related source files.

5. New files `orflib/math/pricers/simplepricers.hpp` and `simplepricers.cpp`.  
	Definition of the functions fwdPrice(), digitalOptionBS() and europeanOptionBS().

6. New file `xlorflib/xlfunctions1.cpp`.  
	Added definition of the following functions:  
	xlOrfErf(), xlOrfInvErf(), xlOrfNormalCdf(), xlOrfNormalInvCdf(), xlOrfFwdPrice(), xlOrfDigiBS() and xlOrfEuroBS().

7. In file `xlorflib/xlregister.cpp`  
	Added registration of Excel callable functions:   
	ORF.ERF, ORF.INVERF, ORF.NORMALCDF, ORF.NORMALINVCDF, ORF.FWDPRICE, ORF.DIGIBS, ORF.EUROBS.

### Modifications

1. Removed unnecessary file `orflib/empty.cpp`


VERSION 0.1.0
-------------

### Additions

1. `orflib-vs15.sln` VS solution file, that contains the projects `orflib` and `xlorflib`.

2. New folder `orflib` with start-up code for the core library.

3. `orflib/orflib-vs15.vcxproj` VC++ project file, that builds the core library `orlib.lib`.

4. New folder `xlorflib` with start-up code for the Excel interface.

5. `xlorflib/xlorflib-vs15.vcxproj` VC++ project file, that builds the `xlorflib.xll` Excel add-in.

6. This release notes file.

7. `.gitignore` file for managing which files to keep under revision control.
