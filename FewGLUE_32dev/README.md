# FewGLUE_32dev

This repository contains the FewGLUE_32dev dataset, an extension of the [FewGLUE](https://github.com/timoschick/fewglue), which enables NLU few-shot learning tasks to be benchmarked under a new 32-sample-dev setting. It has been proved in [previous work](https://arxiv.org/abs/2012.15723) that using larger development sets confer a significant advantage beyond few-shot. FewGLUE_32dev is built by adding additional few-shot dev sets with 32 examples randomly selected from the original/unused SuperGLUE training sets.


### Data Format

All files follows the exact same format as [SuperGLUE task files](https://super.gluebenchmark.com/tasks).

### Structure

For each SuperGLUE task `T`, the directory `FewGLUE_32dev/T` contains 5 files, including the original train/unlabeled files (`train.jsonl`/`unlabeled.jsonl`) from FewGLUE, the original dev/test files (`dev.jsonl`/`test.jsonl`) from SuperGLUE, and the few-shot 32-sample-dev file (`dev32.jsonl`). 


### Citation

If you make use of FewGLUE_32dev, please cite the following paper:

    @article{liu2021gpt,
      title={GPT Understands, Too}, 
      author={Xiao Liu and Yanan Zheng and Zhengxiao Du and Ming Ding and Yujie Qian and Zhilin Yang and Jie Tang},
      year={2021},
      journal={arXiv preprint arXiv:2103.10385},
      url={https://arxiv.org/abs/2103.10385}
    }
