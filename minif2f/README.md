# MiniF2F

## More coming soon...
We have released our validation set, which was used to obtain the results reported in our [second blog post](https://www.harmonic.fun/news#blog-post-2-link). We are planning on releasing the train and test set soon.

## Our Improvements to MiniF2F
To accurately assess our system's capabilities, we have made several improvements to MiniF2F:

1. We translated the problem statements to Lean 4, the leading system for formal mathematics today.
2. We re-split the 488 problems uniformly randomly into a training set of 392 problems, a validation set of 48 problems, and a test set of 48 problems. The new test set and val set are an unbiased random subset of the original test set. The train set is the remaining problems from the original benchmark.
3. We ensured that each formal statement is associated with an accurate natural-language statement, allowing us to evaluate autoformalization capabilities.
4. We fixed many incorrect formalizations, including several theorem statements that became trivial or impossible in their original Lean encodings.

We began with formal statements released by the [Hoskinson Center](https://huggingface.co/datasets/hoskinson-center/minif2f-lean4), themselves derived from [Facebook Research’s fork](https://github.com/facebookresearch/miniF2F) which fixed several issues with the [original benchmark](https://github.com/openai/miniF2).

## MiniF2F

The original version of (MiniF2F from OpenAI)[ https://github.com/openai/miniF2F] provides more context on the original benchmark.

### Citation

The benchmark is described in detail in the following [pre-print](https://arxiv.org/abs/2109.00110):
```
@article{zheng2021minif2f,
  title={MiniF2F: a cross-system benchmark for formal Olympiad-level mathematics},
  author={Zheng, Kunhao and Han, Jesse Michael and Polu, Stanislas},
  journal={arXiv preprint arXiv:2109.00110},
  year={2021}
}
```
