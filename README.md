# deep-learning-model-archtecture-design-advice

## operator fusion

- batchnorm - scale
- convolution - batchnorm
- convolutiondepthwise - batchnorm
- deconvolution - batchnorm
- deconvolutiondepthwise - batchnorm
- innerproduct - batchnorm
- convolution - relu
- convolutiondepthwise - relu
- deconvolution - relu
- deconvolutiondepthwise - relu
- innerproduct - relu

## eliminate noop operator

- innerproduct - dropout
- flatten after global pooling

## prefer better operator

- replace convolution with innerproduct after global pooling

- [model optimize · Tencent/ncnn Wiki](https://github.com/Tencent/ncnn/wiki/model-optimize)
