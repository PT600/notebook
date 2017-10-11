# Chap3

## Regularization
    Regularization can be viewed as a way of compromising between finding small weights and minimizing the original cost function.
    The relative importance of the two elements of the compromise depends on the value of λ: when λ is small we prefer to minimize the original cost function, but when λ is large we prefer small weights.
    When a particular weight has a large magnitude, |w||w|, L1 regularization shrinks the weight much less than L2 regularization does. By contrast, when |w||w| is small, L1 regularization shrinks the weight much more than L2 regularization.

## L1 Regularization
    The net result is that L1 regularization tends to concentrate the weight of the network in a relatively small number of high-importance connections, while the other weights are driven to zero.
