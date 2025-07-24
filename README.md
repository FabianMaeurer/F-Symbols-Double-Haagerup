# F-Symbols for the Double of the Haagerup fusion category

Using the Julia Package [TensorCategories.jl](https://github.com/fabianmaeurer/TensorCategories.jl) we where able to compute the $F$- ans $R$-symbols of the drinfeld double of the fusion category $\mathcal H_3$ comming from the Haagerup subfactor. 
To accomplish this we used the F-symbols for $\mathcal H_3$ computed for the [Anyonwiki](https://anyonwiki.github.io) and fed that to the algorithm we developed in [1].

## The Data
We provid the data in algebraic and numeric form. The solutions in the folders "Double_Haagerup_#_Symbols" are formatted as a csv where the first ten columns $a,b,c,d,e,\alpha,\beta,f,\gamma,\delta$ correspond to the index of the $F$-symbol 
```math 
\left[F_{a,b,c}^d\right]_{f, \delta,\gamma}^{e,\alpha, \beta}
```
are either algerbaic numbers or numeric symbols depending on the folder. The numeric ones are self-explanatory.

### Algebraic Data
The algebraic solutions in the folder "AlgebraicSymbols/Double_Haagerup_#_Symbols" are formatted such that they show a 48-dimensional vector correspponding to the coefficients the standard basis $1,x,...,x^47$ of the Numberfield 
```math
K = \mathbb Q(x), ~~~ 0 = x^48 - x^47 + 2*x^46 - 2*x^45 + 2*x^44 - x^43 - x^42 + 4*x^41 - 8*x^40 + 12*x^39 - 15*x^38 + 15*x^37 - 10*x^36 + 51*x^35 - 31*x^34 + 57*x^33 - 27*x^32 + 2*x^31 + 59*x^30 - 141*x^29 + 229*x^28 - 313*x^27 + 342*x^26 - 285*x^25 + 85*x^24 + 285*x^23 + 342*x^22 + 313*x^21 + 229*x^20 + 141*x^19 + 59*x^18 - 2*x^17 - 27*x^16 - 57*x^15 - 31*x^14 - 51*x^13 - 10*x^12 - 15*x^11 - 15*x^10 - 12*x^9 - 8*x^8 - 4*x^7 - x^6 + x^5 + 2*x^4 + 2*x^3 + 2*x^2 + x + 1
```



---
[1] F. Mäurer, U. Thiel, "Computing the center of a fusion category", [https://arxiv.org/abs/2406.13438](https://arxiv.org/abs/2406.13438)
