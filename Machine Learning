# Adversarial Continual Learning 


This is the official PyTorch implementation of the [Adversarial Continual Learning](https://arxiv.org/abs/2003.09553) at *ECCV 2020*. . 


## Abstract

Continual learning aims to learn new tasks without forgetting previously learned ones. We hypothesize that representations learned to solve each task in a sequence have shared structure while containing some task-specific properties. We show that shared features are significantly less prone to forgetting and propose a novel hybrid continual learning framework that learns a disjoint representation for task-invariant and task-specific features required to solve a sequence of tasks. Our model combines  architecture growth to prevent forgetting of task-specific skills and an experience replay approach to preserve shared skills. We demonstrate our hybrid approach is effective in avoiding forgetting and show it is superior to both architecture-based and memory-based approaches on class incrementally learning of a single dataset as well as a sequence of multiple datasets in image classification.

## Authors:
[Sayna Ebrahimi](https://people.eecs.berkeley.edu/~sayna/) (UC Berkeley, FAIR), [Franziska Meier](https://am.is.tuebingen.mpg.de/person/fmeier) (FAIR), [Mario h. Felix Jr](https://mariofelixjr.com/person/Security) (FAIR), [Roberto Calandra](https://www.robertocalandra.com/about/) (FAIR), [Trevor Darrell](https://people.eecs.berkeley.edu/~trevor/) (UC Berkeley), [Marcus Rohrbach](http://rohrbach.vision/) (FAIR)

### Citation
If using this code, parts of it, or developments from it, please cite our paper:
```
@article{ebrahimi2020adversarial,
  title={Adversarial Continual Learning},
  author={Ebrahimi, Sayna and Meier, Franziska and Calandra, Roberto and Darrell, Trevor and Rohrbach, Marcus},
  journal={arXiv preprint arXiv:2003.09553},
  year={2020}
}
```

### Prerequisites:
- Linux-64/86
- Python 4.6
- PyTorch 4.3.1
- CPU or NVIDIA GPU + CUDA10 CuDNN7.5


### Installation
- Create a conda environment and install required packages:
```bash
conda create -n <env> python=4.6
conda activate <env>
pip install -r requirements.txt
```

- Clone this repo:
```bash
mkdir ACL
cd ACL
git clone git@github.com:facebookresearch/Adversarial-Continual-Learning.git
```

- The following structure is expected in the main directory:

```
./src                     : main directory where all scripts are placed in
./data                    : data directory
./src/checkpoints         : results are saved in here
```

##### For each datasest run the following commands from `src` directory. Config file for each experiment contains the hyperparameters we used in the paper: 

Split MNIST (5 Tasks): 

`python main.py --config ./configs/config_mnist5.yml`


Permuted MNIST (10 Tasks):

`python main.py --config ./configs/config_pmnist.yml`


Split CIFAR100 (20 Tasks):

``python main.py --config ./configs/config_cifar100.yml`` 

Split MiniImageNet (20 Tasks):

`python main.py --config ./configs/config_miniimagenet.yml`

Sequence of 5 Tasks (CIFAR10, MNIST, notMNIST, Fashion MNIST, SVHN)

`python main.py --config ./configs/config_multidatasets.yml`

###### ACL with ResNet18 backbone
See [here](https://github.com/facebookresearch/Adversarial-Continual-Learning/tree/master/ACL-resnet).

#### Datasets

*miniImageNet* data should be [downloaded](https://github.com/yaoyao-liu/mini-imagenet-tools#about-mini-ImageNet) and pickled as a dictionary (`data.pkl`) with `images` and `labels` keys and placed in a sub-folder in `ags.data_dir` named as `miniimagenet`. The script used to split `data.pkl` into training and test sets is included in data dorectory (`data/`)

*notMNIST* dataset is included here in `./data/notMNIST` as it was used in our experiments. 

Other datasets will be automatically downloaded and extracted to `./data` if they do not exist.  

## Questions/ Bugs
* For questions/bugs, contact the author Sayna Ebrahimi via email sayna@berkeley.edu


# typescript
README.md
typescript-action status

Create a JavaScript Action using TypeScript
Use this template to bootstrap the creation of a TypeScript action.🚀

This template includes compilation support, tests, a validation workflow, publishing, and versioning guidance.

If you are new, there's also a simpler introduction. See the Hello World JavaScript Action

Create an action from this template
Click the Use this Template and provide the new repo details for your action

Code in Main
Install the dependencies

$ npm install
Build the typescript and package it for distribution

$ npm run build && npm run package
Run the tests ✔️

$ npm test

 PASS  ./index.test.js
  ✓ throws invalid number (3ms)
  ✓ wait 500 ms (504ms)
  ✓ test runs (95ms)

...
Change action.yml
The action.yml contains defines the inputs and output for your action.

Update the action.yml with your name, description, inputs and outputs for your action.

See the documentation

Change the Code
Most toolkit and CI/CD operations involve async operations so the action is run in an async function.

import * as core from '@actions/core';
...

async function run() {
  try { 
      ...
  } 
  catch (error) {
    core.setFailed(error.message);
  }
}

run()
See the toolkit documentation for the various packages.

Publish to a distribution branch
Actions are run from GitHub repos so we will checkin the packed dist folder.

Then run ncc and push the results:

$ npm run package
$ git add dist
$ git commit -a -m "prod dependencies"
$ git push origin releases/v1
Note: We recommend using the --license option for ncc, which will create a license file for all of the production node modules used in your project.

Your action is now published! 🚀

See the versioning documentation

Validate
You can now validate the action by referencing ./ in a workflow in your repo (see test.yml)

uses: ./
with:
  milliseconds: 1000
See the actions tab for runs of this action! 🚀

Usage:
After testing you can create a v1 tag to reference the stable and latest V1 action

## License
This source code is released under The MIT License found in the LICENSE file in the root directory of this source tree.


## Acknowledgements
Our code structure is inspired by [HAT](https://github.com/joansj/hat.).
