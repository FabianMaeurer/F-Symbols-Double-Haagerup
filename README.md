# F-Symbols for the Double of the Haagerup fusion category

Using the Julia Package [TensorCategories.jl](https://github.com/fabianmaeurer/TensorCategories.jl) we where able to compute the $F$- ans $R$-symbols of the drinfeld double of the fusion category $\mathcal H_3$ comming from the Haagerup subfactor. 
To accomplish this we used the F-symbols for $\mathcal H_3$ computed for the [Anyonwiki](https://anyonwiki.github.io) and fed that to the algorithm we developed in [1].

## The Data
We provid the data in algebraic and numeric form. The solutions in the folders "Double_Haagerup_#_Symbols" are formatted as a csv where the first ten columns $a,b,c,d,f,\gamma,\delta,e,\beta,\alpha$ correspond to the index of the $F$-symbol 
```math 
\left[F_{a,b,c}^d\right]_{f, \delta,\gamma}^{e,\alpha, \beta}
```
are either algerbaic numbers or numeric symbols depending on the folder. The numeric ones are self-explanatory.

### Algebraic Data
The algebraic solutions in the folder "AlgebraicSymbols/Double_Haagerup_#_Symbols" are formatted such that they show a 48-dimensional vector correspponding to the coefficients the standard basis $1,x,...,x^{47}$ of the Numberfield 
```math
K = \mathbb Q(x), ~~~ 0 = x^{48} - x^{47} + 2x^{46} - 2x^{45} + 2x^{44} - x^{43} - x^{42} + 4x^{41} - 8x^{40} + 12x^{39} - 15x^{38} + 15x^{37} - 10x^{36} + 51x^{35} - 31x^{34} + 57x^{33} - 27x^{32} + 2x^{31} + 59x^{30} - 141x^{29} + 229x^{28} - 313x^{27} + 342x^{26} - 285x^{25} + 85x^{24} + 285x^{23} + 342x^{22} + 313x^{21} + 229x^{20} + 141x^{19} + 59x^{18} - 2x^{17} - 27x^{16} - 57x^{15} - 31x^{14} - 51x^{13} - 10x^{12} - 15x^{11} - 15x^{10} - 12x^{9} - 8x^{8} - 4x^{7} - x^{6} + x^{5} + 2x^{4} + 2x^{3} + 2x^{2} + x + 1
```

## In TensorCategories.jl

The data is also available in the Julia package [TensorCategories.jl](https://github.com/fabianmaeurer/TensorCategories.jl) where they were computed. 

```julia
julia> using TensorCategories

julia> C = haagerup_H3_center()
Center of fusion category HI(Z3)
```


---
[1] F. Mäurer, U. Thiel, "Computing the center of a fusion category", [https://arxiv.org/abs/2406.13438](https://arxiv.org/abs/2406.13438)
