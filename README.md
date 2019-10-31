# rpf-pytorch
This is my [PyTorch](https://pytorch.org/) re-implementaion of the code accompanying the paper
[Randomized Prior Functions for Deep Reinforcement Learning](https://arxiv.org/abs/1806.03335)
by me.

You can play it in
[this google collaboratory link](https://colab.research.google.com/github/kngwyu/rpf-pytorch/blob/master/rpf_pytorch.ipynb)
.

Plese see the
[author's website](https://sites.google.com/corp/view/randomized-prior-nips-2018/home)
for detail and the original code.


## Caveats
My RPF DQN re-implementaion works well but **more poorly** than the author's
result left in the notebook.

And it looks **the result is unstable** in that the expectated number of episodes
it needs to get plus return has high variance(1200~3000 episodes).

So there's some possible reasons for that, say,
- My implementaion is incorrect
- Some insignificant implementaion differences like initialization

But I think this result shows that **we must get lucky** for success
, even if we use nice exploration-exploitation algorithms such as RPF.
