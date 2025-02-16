### Bagged FSR: Rehabilitating Forward Stepwise Regression

"Forward Stepwise Regression (FSR) is hardly used today. That is mostly because regularization is a better way to think about variable selection. However, part of the reason for its disuse is that FSR is a greedy optimization strategy with unstable paths. Jigger the data a little, and the search paths, variables in the final set, and the performance of the final model can all change dramatically. The same issues, however, affect another greedy optimization strategy—CART. The insight that rehabilitated CART was bagging—building multiple trees using random subspaces (sometimes on randomly sampled rows) and averaging the results. What works for CART should principally also work for FSR. If you are using FSR for prediction, you can build multiple FSR models using random subspaces and random samples of rows and then average the results. If you are using it for variable selection, you can pick variables with the highest batting average (n_selected/n_tried). (LASSO will beat it on speed, but there is little reason to expect that it will beat it on results.)"

Via https://gojiberries.io/2019/11/06/rehabilitating-forward-stepwise-regression/


See [simulation results](https://htmlpreview.github.io/?https://github.com/soodoku/bagged_fsr/blob/main/bagged_fsr.html)
