# Why ReLU

    * 第一，采用sigmoid等函数，算激活函数时（指数运算），计算量大，反向传播求误差梯度时，求导涉及除法，计算量相对大，而采用Relu激活函数，整个过程的计算量节省很多。
    * 第二，对于深层网络，sigmoid函数反向传播时，很容易就会出现梯度消失的情况（在sigmoid接近饱和区时，变换太缓慢，导数趋于0，这种情况会造成信息丢失，参见 @Haofeng Li  答案的第三点），从而无法完成深层网络的训练。
    * 第三，Relu会使一部分神经元的输出为0，这样就造成了网络的稀疏性，并且减少了参数的相互依存关系，缓解了过拟合问题的发生（以及一些人的生物解释balabala）。

    ** 一旦神经元与神经元之间改为线性激活，网络的非线性部分仅仅来自于神经元部分选择性激活。**

## Referrers
    * [Why ReLU work](http://shuokay.com/2016/10/01/why-relu-work/)
    * [ReLu(Rectified Linear Units)激活函数](http://www.cnblogs.com/neopenx/p/4453161.html)
    * [请问人工神经网络中的activation function的作用具体是什么？为什么ReLu要好过于tanh和sigmoid function?] (https://www.zhihu.com/question/29021768)
