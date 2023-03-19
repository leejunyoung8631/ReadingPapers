ReadingPapers
read papers with simple comments
==========================


useful github
-----------------------------
1. https://github.com/DaoSword/Time-Series-Forecasting-and-Deep-Learning
2. https://github.com/heejkoo/Awesome-Diffusion-Models#generation-3


Time series forecasting
-----------------------------

* Less Is More: Fast Multivariate Time Series Forecasting with Light Sampling-oriented MLP Structures
    * arsiv, 2022
> - propose LightTS   
> - MLP-based model -> IEBlock(bottleneck based mlp model)   
> - Phase 1    
>   continuous sampling for local, inteval sampling for global   
>	process 1 : 데이터를 continuous 한 길이로 자름   
>	process 2 : 특정 inteval한 간격으로 데이터를 모아서 자름   
>	이후, IEBlock 으로 같은 feature 내의 관계 찾기   
> - Phase 2    
>   Interdepedencies beween different feature   
>   phase1의 feature를 concat & reshape   
>   IEBlock으로 다른 feature간의 관계를 얻기   

