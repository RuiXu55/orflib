ORFLIB Release Notes
====================

VERSION 0.4.0
-------------

### Additions

1. New file `orflib/sptrmap.hpp`
	It defines the SPtrMap class template.

2. New folder `orflib/market` with two new files `yieldcurve.hpp` and `yieldcurve.cpp`.  
	They define and implement the YieldCurve class.

3. Two new files `orflib/market/market.hpp` and `market.cpp`  
	They define and implement the Market singleton class.

4. New files `orflib/util.hpp` for generic utility fiunctions.   
	It contains a function for trimming strings
	
5. Two new utility functions xlAddTick() and xlStripTick() in files `xlorflib/xlutils.hpp` and `.cpp`.  
	These are used for adding and removing the tick-tock mark after the name of the object handle.

6. Two new files `xlorflib/xlfunctions2.cpp` and `xlorflib/xlregister2.cpp`  
	They implement and register the following Excel functions  
	ORF.MKTLIST  
	ORF.MKTCLEAR  
	ORF.YCCREATE  
	ORF.DF  
	ORF.FWDDF  
	ORF.SPOTRATE  
	ORF.FWDRATE  


VERSION 0.3.0
-------------

### Additions

1. New file `orflib/math/matrix.hpp`.   
  It defines aliases for the Vector and Matrix classes to be used in numerical work.

2. New folder `orflib/math/interpol` with two new files `piecewisepolynomial.hpp` and `piecewisepolynomial.cpp`.  
	They implement the class PiecewisePolynomial.

3. Two new files `xlorflib/xlutils.hpp` and `xlorflib/xlutils.cpp`.  
	They implement the utility functions xlOperToVector(), xlVectorToOper(), xlOperToMatrix() and xlMatrixToOper().
	
4. The following Excel callable functions have been added:  
	ORF.MATRIXECHO  
	ORF.PPOLYEVAL  
	ORF.PPOLYINTEGRAL  
	ORF.PPOLYSUM  
	These are used for testing the Matrix and PiecewisePolynomial classes.

### Modifications

1. Orflib now has dependency on the armadillo C++ matrix library. 
  The "C/C++->Additional Include Directories" project settings have been updated.


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
	Definition of the functions fwdPrice() and digitalOptionBS().

6. New file `xlorflib/xlfunctions1.cpp`.  
	Added definition of the following functions:  
	xlOrfErf(), xlOrfInvErf(), xlOrfNormalCdf(), xlOrfNormalInvCdf(),
	xlOrfFwdPrice() and xlOrfDigiBS().

7. In file `xlorflib/xlregister.cpp`  
	Added registration of Excel callable functions:   
	ORF.ERF, ORF.INVERF, ORF.NORMALCDF, ORF.NORMALINVCDF, ORF.FWDPRICE, ORF.DIGIBS.

### Modifications

1. Removed unnecessary file `orflib/emptystub.cpp`


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
