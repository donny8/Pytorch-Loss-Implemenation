# Pytorch-Loss-Implementation
Implemented pytorch BCELoss, CELoss and customed-BCELoss-with-Label-Smoothing

The python implementations of torch BCELoss and CELoss are for the understanding how they work.

After pytorch `0.1.12` , as you know, there is `label smoothing` option, only in [CrossEntropy loss](https://pytorch.org/docs/stable/generated/torch.nn.CrossEntropyLoss.html#torch.nn.CrossEntropyLoss) 

It is possible to consider binary classification as 2-class-classification and apply CE loss with label smoothing.

But I did not want to convert input shape as (2, batch) and target's `dtype`.

So I implemented `label smoothing` to BCE loss by myself, which means there could be some error.

Since I'd found this customed BCE with `label smoothing` helped improve the model performance, I would like to share with you.

I hope it also works in your project.

If anyone find some error, please share your opinion and let me improve the code.
