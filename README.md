#	Introduction

This asset will provide access to the MathNET Numerics Special Functions library. It is part of a series of assets that will offer complimentary mathematical functionality to what is currently possible with Blue Prism alone.

## Prerequisites
To use this asset, you require a licenced Blue Prism installation or trial. More information on Blue Prism can be found here. https://www.blueprism.com.

You will also require to download the MathNET. Numerics dll from NuGet. The library is found at https://www.nuget.org/packages/MathNet.Numerics/

This asset provides 39 mathematical functions. Please see the table of contents for the extensive list.
 
## Configuration
The asset is downloaded from the Digital Exchange (DX) It is installed int the usual manner using the import item from the file menu.

The bprelease file contains:
•	Utility MathsNET – Special Functions
•	Process Example – MathsNet – Special Functions

You will also be required to download the MathNET. Numerics dll from NuGet. It can be found at https://www.nuget.org/packages/MathNet.Numerics/
It needs to be installed in your Blue Prism directory, which will depend on your specific installation. If your Blue Prism is a default install, then the location for its deployment is

C:\program files\Blue Prism Limited\Blue Prism Automate

 


 
## Using the Asset
This asset is intended to assist anyone requiring extended mathematical functionality beyond the base of what exists in Blue Prism, by default.

### Factorial
The factorial function is a multiplication of all the values up to the xParameter. So if x is 5, the factorial(5) is 5x4x3x2x1 = 120.
The factorial equation
:  
#### Input:

Name|Description|Data Type
|---|-----------|---------|
|xParameterValue|The value of which to determine the factorial.|Number|

#### Output:
Name|Description|Data Type 
|---|-----------|---------|
|Result|The resulting factorial value|Number|
|ResultText|The resulting factorial value where numerical limits are exceeded.|Text|

### Logarithmic Factorial Function
Computes the logarithmic factorial function. Parameter must be > 0.
 
#### Input: 
Name| 	Description| 	Data Type
|---|-----------|---------|
ParameterValue| 	The input value to calculate the logarithmic factorial.|	Text 
#### Output: 
Name| 	Description| 	Data Type
|---|-----------|---------|
Result| 	The resulting value. |	Number

 
###	Binomial Coefficient
The binomial coefficient is the number of ways of picking k unordered outcomes from n possibilities. This is sometimes known as combinatorics. (source https://en.wikipedia.org/wiki/Binomial_coefficient)
 
#### Input:
Name |	Description |	Data Type 
|---|-----------|---------|
nParameterValue |	The number of elements.| 	Number
kParameterValue|	The number of unordered elements of the subset.|	Number

#### Output:
Name| 	Description| 	Data Type |
|---|-----------|---------|
Result| 	The resulting coefficient.|	Number|

###	BinomialLn
Computes the natural logarithm of the binomial coefficient. Ln(n choose k).
 
#### Input:
Name| 	Description| 	Data Type |
|---|-----------|---------|
nParameterValue| 	The number of elements. |	Number|
kParameterValue|	The number of unordered elements of the subset.|	Number

#### Output:
Name| 	Description |	Data Type |
|---|-----------|---------|
Result| 	The resulting natural logarithm of the coefficient.|	Number

### Multinomial
A statistical experiment that consist of n repeated trials. Each trial has a discrete number of possible outcomes. On any given trial, the probability that a particular outcome will occur is constant.
 
#### Input:
Name| 	Description| 	Data Type |
|---|-----------|---------|
nParameterValue| 	The number of elements.| 	Number
niParameterValue|	The number of unordered elements of the subset.|	Number

#### Output:
Name |	Description |	Data Type |
|---|-----------|---------|
Result |	The resulting coefficient.|	Number


###	Exponential Integral
The exponential integral is a special function on the complex plane. It is defined as one particular definite integral of the ratio between an exponential function and its argument.
 
#### Input:
Name |	Description |	Data Type 
|---|-----------|---------|
nParameterValue |	The number of elements. |	Number
niParameterValue|	The number of unordered elements of the subset.|	Number
#### Output:
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting coefficient.|	Number

###	Gamma Function
The gamma function is an extension of the factorial function to complex numbers. The gamma function is defined for all complex numbers except negative integers.
 
#### Input: 
Name| 	Description| 	Data Type 
|---|-----------|---------|
zParameterValue| 	The input value to apply to the gamma function|	Number 
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result| 	The resulting gamma value.| 	Number

###	GammaLn Function
The gammaln function will return the natural logarithm of the gamma function, using zParameterValue which must be positive.
 
#### Input: 
Name| 	Description |	Data Type 
|---|-----------|---------|
zParameterValue |	The input value to apply to the gamma function.|	Number 
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting gamma value. |	Number

###	Gamma Lower Incomplete (Unregularized)
The lower incomplete gamma function is a special function that is a solution to various mathematical problems such as integrals. The lower incomplete gamma is defined as an integral from zero to a variable upper limit.
Returns the lower incomplete gamma function gamma(a,x) = int(exp(-t)t^(a-1),t=0..x) for real a>0, x>0.
 
#### Input: 
Name| 	Description |	Data Type 
|---|-----------|---------|
aParameterValue| 	Complex parameter. Real part is positive.|	Number 
xParameterValue|	Complex parameter. Real part is positive.| Number	
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting gamma value. |	Number

### Gamma Upper Incomplete (Unregularized)
The upper incomplete gamma function is a special function that is a solution to various mathematical problems such as integrals. The upper incomplete gamma is defined as an integral from zero to infinity.
Returns the upper incomplete gamma function gamma(a,x) = int(exp(-t)t^(a-1),t=0..x) for real a>0, x>0.
 
#### Input: 
Name |	Description |	Data Type 
aParameterValue |	Complex parameter. Real part is positive.|	Number 
xParameterValue|	Complex parameter. Real part is positive.| Number	
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting gamma value.| 	Number

### Gamma Lower Incomplete (Regularized)
Returns the lower incomplete regularized gamma function P(a,x) = 1/Gamma(a) * int(exp(-t)t^(a-1),t=0..x) for real a>0,x>0.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
aParameterValue |	Complex parameter. Real part is positive.|	Number 
xParameterValue	|Complex parameter.| Real part is positive.	
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting gamma value. |	Number

### Gamma Upper Incomplete (Regularized)
The upper incomplete gamma function is a special function that is a solution to various mathematical problems such as integrals. The upper incomplete gamma is defined as an integral from zero to infinity.
 
#### Input: 
Name |	Description |	Data Type
|---|-----------|---------|
aParameterValue |	Complex parameter. Real part is positive.|	Number 
xParameterValue|	Complex parameter. Real part is positive.|	Number
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting gamma value. |	Number

### Gamma Lower Incomplete (Regularized Inverse)
Returns the inverse P^(-1) of the regularized lower incomplete regularized gamma function P(a,x) = 1/Gamma(a) * int(exp(-t)t^(a-1),t=0..x) for real a>0,x>0, such that P^(-1)(a,P(a,x)) == x.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
aParameterValue |	Complex parameter. Real part is positive.|	Number 
xParameterValue|	Complex parameter. Real part is positive.|	Number
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting gamma value.| 	Number

###	DiGamma
Computes the Digamma function which is mathematically defined as the derivative of the logarithm of the gamma function. This implementation is based on Jose Bernardo Algorithms AS 103: Psi (Digamma) Function, Applied Statistics, Volume 25 Number 3, 1976, pages 315-317.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
aParameterValue |	Complex parameter. Real part is positive.|	Number 
xParameterValue|	Complex parameter. Real part is positive.|	Number
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting Digamma value. |	Number

###	DiGamma Inverse
Computes the inverse Digamma function: This is the inverse of the logarithm of the gamma function. This function will only return solutions that are positive. This implementation is based on the bisection method. https://en.wikipedia.org/wiki/Digamma_function

#### Input: 
Name |	Description |	Data Type
|---|-----------|---------|
aParameterValue |	Integer parameter. Real part is positive.|	Number 
xParameterValue|	Integer parameter. Real part is positive.|	Number
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting Digamma value.| 	Number

### Euler Beta Function
Computes the Euler Beta function. https://en.wikipedia.org/wiki/Beta_function

#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
zParameterValue |	Floating Point Value|	Number 
wParameterValue|	Floating Point Value|	Number

#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result| 	The resulting beta value.| 	Number

###	Euler BetaLn Function
Computes the natural logarithm of the  Euler Beta function, evaluated at z,w. https://en.wikipedia.org/wiki/Beta_function
  
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
zParameterValue |	Floating Point Value|	Number 
wParameterValue	|Floating Point Value|	Number
#### Output: 
Name |	Description |	Data Type 
Result| 	The resulting BetaLn value. |	Number

###	Incomplete Beta (Unregularized)
Returns the lower incomplete (unregularized) beta function B(a,b,x) = int(t^(a-1)*(1-t)^(b-1),t=0...x) for real a>0, b>0, 1>=x>=0.. https://en.wikipedia.org/wiki/Beta_function#Incomplete_beta_function
 
#### Input:
Name |	Description |	Data Type 
|---|-----------|---------|
aParameterValue |	Floating Point Value.|	Number 
bParameterValue|	Floating Point Value|	Number
xParameterValue|	Floating Point Value|	Number

#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result| 	The resulting gamma value.| 	Number

###	Beta Regularized
Returns the regularized lower incomplete beta function I_x(a,b) = 1/Beta(a,b) * int(t^(a-1)*(1-t)^(b-1),t=0...x) for real a>0, b>0, 1>=x>=0.. https://en.wikipedia.org/wiki/Beta_function
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
aParameterValue |	Floating Point Value|	Number 
bParameterValue|	Floating Point Value|	Number
xParameterValue|	Floating Point Value|	Number
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting beta value. |	Number

###	Error Function
Calculates the Error Function. https://en.wikipedia.org/wiki/Error_function
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
zParameterValue |	Floating Point Value|	Number 
#### Output: 
Name| 	Description |	Data Type 
|---|-----------|---------|
Result| 	The resulting error value.| 	Number

###	Complimentary Error Function
Returns the complimentary error function evaluated at given value z.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
zParameterValue |	Floating Point Value|	Number 
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result| 	The resulting complimentary error function value. |	Number


###	Complimentary Inverse Error Function
Calculates the complimentary Inverse Error Function evaluated at z.. https://en.wikipedia.org/wiki/Error_function
 
#### Input: 
Name |	Description |	Data Type
|---|-----------|---------|
zParameterValue |	Floating Point Value|	Number 
#### Output: 
Name| 	Description |	Data Type 
|---|-----------|---------|
Result 	|The resulting error value.| 	Number

###	Logistic Function
Returns the logistic function. https://en.wikipedia.org/wiki/Logistic_function
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
xParameterValue |	Floating Point Value|	Number 
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting complimentary error function value. |	Number


###	Logit Function
Calculates the Inverse of the logistic function.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
yParameterValue |	For y between 0 and 1 (where the function is real valued).|	Number 
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting logit value. |	Number

 
###	Harmonic
Computes the t’th harmonic value.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
tParameterValue |	Integer Value|	Number 
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting harmonic value. |	Number


###	Compute the Generalised Harmonic
Compute the generalized harmonic number of order n of m. (1+1/2^m+1/3m+....1/n^m)
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
nParameterValue |	Integer Value|	Number 
mParameterValue|	Floating Point Value| Number	
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting error value.| 	Number

 
###	Bessell I0
Returns the modified Bessel function of first kind, order 0 of the argument. The function is defined as i0(x) = j0(ix). The range is partioned into the two intervals [0,8] and [8,infinity]. Chebyshev polynomial expansions are employed in each interval.
 
#### Input: 
Name |	Description |	Data Type 
xParameterValue |	Floating Point Value|	Number 
#### Output: 
Name |	Description |	Data Type 
Result| 	The resulting Bessell I0 function value.| 	Number


###	Bessell I1
Returns the modified Bessel function of first kind, order 1 of the argument. The function is defined as i1(x) = -i  j1(ix). The range is partioned into the two intervals [0,8] and [8,infinity]. Chebyshev polynomial expansions are employed in each interval.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
xParameterValue |	Floating Point Value|	Number 
#### Output: 
Name |	Description |	Data Type
|---|-----------|---------|
Result |	The resulting Bessell I1 function value. |	Number

 
###	Bessell K
Returns the modified Bessel function of the second kind. BesselK(n,z) is a solution to the modified Bessel differential equation.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
nParameterValue |	Floating Point Value|	Number 
zParameterValue|	Floating Point Value|	Number
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result 	|The resulting Bessel K function value.| 	Number

###	Bessell K0
Returns the modified Bessel function of the second kind, order 0 of the argument. The range is partitioned into the two intervals [0,8] and [8, infinity]. Chebyshev polynomial expansions are employed in each interval.
 
#### Input: 
Name |	Description |	Data Type
|---|-----------|---------|
xParameterValue |	Floating Point Value|	Number 
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result| 	The resulting Bessel I1 function value. |	Number

###	Bessell K0e
Returns the modified Bessel function of the second kind. BesselK(n,z) is a solution to the modified Bessel differential equation.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
nParameterValue |	Floating Point Value|	Number 
zParameterValue|	Floating Point Value|	Number
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result| 	The resulting Bessel K function value.| 	Number

###	Bessell K1
Returns the modified Bessel function of the second kind order 1 of the argument. The range is partitioned into the two intervals [0,2] and (2,Infinity). Chebyshev polynomial expansions are employed in each interval.
 
#### Input: 
Name |	Description |	Data Type
|---|-----------|---------|
xParameterValue |	Floating Point Value|	Number 
#### Output: 
Name |	Description |	Data Type
|---|-----------|---------|
Result |	The resulting Bessel I1 function value. |	Number

###	Bessell K1e
Returns the modified Bessel function of the second kind. 
 
#### Input: 
Name |	Description |	Data Type 
nParameterValue |	Floating Point Value|	Number 
zParameterValue|	Floating Point Value|	Number
#### Output: 
Name |	Description |	Data Type 
Result| 	The resulting Bessell K function value. |	Number

### Struve L0
Returns the modified Struve function of order 0.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
xParameterValue |	Floating Point Value|	Number 
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result |	The resulting Struve L0 function value. |	Number

###	Struve L1
Returns the modified Struve function of order 1.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
xParameterValue |	Floating Point Value|	Number 
#### Output: 
Name |	Description |	Data Type
|---|-----------|---------|
Result |	The resulting Bessell K function value. |	Number

###	Bessel L0 Struve L0
Returns the difference between the Bessel I0 and Struve L0 functions.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
xParameterValue |	Floating Point Value|	Number 
#### Output: 
Name |	Description |	Data Type
|---|-----------|---------|
Result |	The resulting Bessell I1 function value. |	Number

###	Bessel I0M Struve L0
Returns the modified Struve function of order 1.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
xParameterValue |	Floating Point Value|	Number 
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result| 	The resulting Bessell K function value. |	Number

###	Bessel I1M Struve L0
Returns the difference between the Bessel I1 and Struve L1 functions.
 
#### Input: 
Name |	Description |	Data Type 
|---|-----------|---------|
xParameterValue |	Floating Point Value|	Number 
#### Output: 
Name |	Description |	Data Type 
|---|-----------|---------|
Result| 	The resulting Bessell I1 function value. |	Number

###	Support
This asset is provided free-of-charge by Blue Prism. Blue Prism does not provide formal support of this asset. Please direct any questions you have, related to this asset, to the Digital Exchange Community page:
https://community.blueprism.com/communities/community-home?CommunityKey=1e516cfe-4d1f-4de9-a9eb-58d15bf38c81

