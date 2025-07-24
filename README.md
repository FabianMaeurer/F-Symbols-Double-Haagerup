# F-Symbols for the Double of the Haagerup fusion category

Using the Julia Package [TensorCategories.jl](https://github.com/fabianmaeurer/TensorCategories.jl) we where able to compute the $F$- ans $R$-symbols of the drinfeld double of the fusion category $\mathcal H_3$ comming from the Haagerup subfactor. 
To accomplish this we used the F-symbols for $\mathcal H_3$ computed for the [Anyonwiki](https://anyonwiki.github.io) and fed that to the algorithm we developed in [^fn1].

## The Dataformat

The Numeric solutions in the folder "Double_Haagerup_#_Symbols" are formatted as a csv where the first ten columns ´´´a,b,c,d,e,\alpha,\beta,f,\gamma,\delta``` correspond to the index of the $F$-symbol $$\left[F_{a,b,c}^d\right]_{f, \delta,\gamma}^{e,\alpha, \beta}.$$
and the last value is a numeric approximation.

[^fn1] F. Mäurer, U. Thiel, "Computing the center of a fusion category", [https://arxiv.org/abs/2406.13438](https://arxiv.org/abs/2406.13438)
