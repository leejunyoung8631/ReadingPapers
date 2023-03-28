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
    * arxiv, 2022
    * Recommendation : ⭐⭐
> - propose model named LightTS   
> - MLP-based model -> IEBlock(bottleneck based mlp model)   
> - Phase 1    
>   continuous sampling for local, inteval sampling for global   
>	process 1 : 데이터를 continuous 한 길이로 자름   
>	process 2 : 특정 inteval한 간격으로 데이터를 모아서 자름   
>	이후, IEBlock 으로 같은 feature 내의 관계 찾기   
> - Phase 2    
>   Interdepedencies beween different feature   
>   phase1의 feature를 concat & reshape   
>   IEBlock으로 다른 feature간의 관계를 습득
> 
> - 대부분 timeseries forecasting은 transformer 기반 모델을 이용하는데, MLP를 이용하여 구현하려는 모델
> - long time inference에서 MLP가 정말로 그 복잡한 데이터의 관계성을 학습할 수 있는지 확인해볼 필요가 있음






Generative model
-----------------------------

* Autoregressive Image Generation using Residual Quantization
    * CVPR, 2022
    * Recommendation : ⭐⭐⭐
> - apply RQ(Residual quantized) to VAE, Transformer
> - 기존 vector quantization 기법에서 codebook과 latent vector size의 tradeoff 문제를 개선 
> - 일반적인 VQ 보다, latent vector의 해상도를 더 낮추며 성능도 좋음.
> - latent vector의 차원을 4개로 확장하여, 4개의 벡터의 합이 이미지의 latent feature를 나타내는 residual 기법을 사용(하나의 vector로 표현하는 것보다 summed 된 vector가 더 효과적)
> - latent vector를 바탕으로 autoregressive spatial, depth transformer를 학습시키고, 이를 이미지 생성시에 사용해서 공간적 정보를 담음.







