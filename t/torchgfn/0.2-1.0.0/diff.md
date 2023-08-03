# Comparing `tmp/torchgfn-0.2.tar.gz` & `tmp/torchgfn-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchgfn-0.2.tar", max compression
+gzip compressed data, was "torchgfn-1.0.0.tar", max compression
```

## Comparing `torchgfn-0.2.tar` & `torchgfn-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0    14346 2023-05-30 14:17:28.832385 torchgfn-0.2/README.md
--rw-r--r--   0        0        0     3204 2023-05-30 14:17:28.832830 torchgfn-0.2/pyproject.toml
--rw-r--r--   0        0        0      217 2023-05-30 14:25:24.260364 torchgfn-0.2/src/gfn/__init__.py
--rw-r--r--   0        0        0      103 2023-05-30 14:17:27.272751 torchgfn-0.2/src/gfn/containers/__init__.py
--rw-r--r--   0        0        0     2153 2023-05-03 09:42:02.656970 torchgfn-0.2/src/gfn/containers/base.py
--rw-r--r--   0        0        0     3584 2023-05-30 14:17:27.272875 torchgfn-0.2/src/gfn/containers/replay_buffer.py
--rw-r--r--   0        0        0    13197 2023-05-30 14:17:27.272991 torchgfn-0.2/src/gfn/containers/states.py
--rw-r--r--   0        0        0    11797 2023-05-30 14:17:27.273148 torchgfn-0.2/src/gfn/containers/trajectories.py
--rw-r--r--   0        0        0     7389 2023-05-30 14:17:27.273305 torchgfn-0.2/src/gfn/containers/transitions.py
--rw-r--r--   0        0        0     3593 2023-05-30 14:17:27.273426 torchgfn-0.2/src/gfn/distributions.py
--rw-r--r--   0        0        0       95 2023-05-30 14:17:27.273545 torchgfn-0.2/src/gfn/envs/__init__.py
--rw-r--r--   0        0        0     7424 2023-05-30 14:17:27.273669 torchgfn-0.2/src/gfn/envs/discrete_ebm.py
--rw-r--r--   0        0        0     8212 2023-05-30 14:17:27.273791 torchgfn-0.2/src/gfn/envs/env.py
--rw-r--r--   0        0        0     8634 2023-05-30 14:17:27.274056 torchgfn-0.2/src/gfn/envs/hypergrid.py
--rw-r--r--   0        0        0      125 2022-11-08 17:34:55.632486 torchgfn-0.2/src/gfn/envs/preprocessors/__init__.py
--rw-r--r--   0        0        0     1852 2023-05-30 14:17:27.274298 torchgfn-0.2/src/gfn/envs/preprocessors/base.py
--rw-r--r--   0        0        0     2268 2023-05-30 14:17:27.274443 torchgfn-0.2/src/gfn/envs/preprocessors/hot.py
--rw-r--r--   0        0        0     6545 2023-05-30 14:17:27.274599 torchgfn-0.2/src/gfn/estimators.py
--rw-r--r--   0        0        0      481 2023-04-28 10:00:41.421203 torchgfn-0.2/src/gfn/losses/__init__.py
--rw-r--r--   0        0        0     9125 2023-05-30 14:17:27.274753 torchgfn-0.2/src/gfn/losses/base.py
--rw-r--r--   0        0        0     6150 2023-05-30 14:17:27.274902 torchgfn-0.2/src/gfn/losses/detailed_balance.py
--rw-r--r--   0        0        0     4939 2023-05-30 14:17:27.275035 torchgfn-0.2/src/gfn/losses/flow_matching.py
--rw-r--r--   0        0        0    14025 2023-05-30 14:17:27.275192 torchgfn-0.2/src/gfn/losses/sub_trajectory_balance.py
--rw-r--r--   0        0        0     3703 2023-05-30 14:17:27.275333 torchgfn-0.2/src/gfn/losses/trajectory_balance.py
--rw-r--r--   0        0        0     5330 2023-05-30 14:17:27.275429 torchgfn-0.2/src/gfn/modules.py
--rw-r--r--   0        0        0      172 2023-05-30 14:17:27.275544 torchgfn-0.2/src/gfn/samplers/__init__.py
--rw-r--r--   0        0        0     5479 2023-05-30 14:17:27.275690 torchgfn-0.2/src/gfn/samplers/actions_samplers.py
--rw-r--r--   0        0        0     4705 2023-05-30 14:17:27.275816 torchgfn-0.2/src/gfn/samplers/trajectories_sampler.py
--rw-r--r--   0        0        0     3383 2023-05-30 14:17:27.275897 torchgfn-0.2/src/gfn/utils.py
--rw-r--r--   0        0        0    15889 1970-01-01 00:00:00.000000 torchgfn-0.2/PKG-INFO
+-rw-r--r--   0        0        0    13343 2023-08-03 19:39:03.617832 torchgfn-1.0.0/README.md
+-rw-r--r--   0        0        0     3279 2023-08-03 17:51:53.277831 torchgfn-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-08-02 13:35:46.365774 torchgfn-1.0.0/src/gfn/__init__.py
+-rw-r--r--   0        0        0     6960 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/actions.py
+-rw-r--r--   0        0        0      116 2023-08-02 13:35:46.365774 torchgfn-1.0.0/src/gfn/containers/__init__.py
+-rw-r--r--   0        0        0     1882 2023-08-02 13:35:46.365774 torchgfn-1.0.0/src/gfn/containers/base.py
+-rw-r--r--   0        0        0     4082 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/containers/replay_buffer.py
+-rw-r--r--   0        0        0    10967 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/containers/trajectories.py
+-rw-r--r--   0        0        0     7964 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/containers/transitions.py
+-rw-r--r--   0        0        0    11633 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/env.py
+-rw-r--r--   0        0        0      291 2023-08-02 13:35:46.365774 torchgfn-1.0.0/src/gfn/gflownet/__init__.py
+-rw-r--r--   0        0        0     6574 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/gflownet/base.py
+-rw-r--r--   0        0        0     7519 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/gflownet/detailed_balance.py
+-rw-r--r--   0        0        0     5351 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/gflownet/flow_matching.py
+-rw-r--r--   0        0        0    12963 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/gflownet/sub_trajectory_balance.py
+-rw-r--r--   0        0        0     2798 2023-08-02 13:35:46.365774 torchgfn-1.0.0/src/gfn/gflownet/trajectory_balance.py
+-rw-r--r--   0        0        0      113 2023-08-02 13:35:46.375774 torchgfn-1.0.0/src/gfn/gym/__init__.py
+-rw-r--r--   0        0        0     4184 2023-08-02 13:35:46.375774 torchgfn-1.0.0/src/gfn/gym/box.py
+-rw-r--r--   0        0        0     9002 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/gym/discrete_ebm.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:35:46.375774 torchgfn-1.0.0/src/gfn/gym/helpers/__init__.py
+-rw-r--r--   0        0        0    30824 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/gym/helpers/box_utils.py
+-rw-r--r--   0        0        0     2179 2023-08-02 13:35:46.375774 torchgfn-1.0.0/src/gfn/gym/helpers/preprocessors.py
+-rw-r--r--   0        0        0     3178 2023-08-02 13:35:46.375774 torchgfn-1.0.0/src/gfn/gym/helpers/test_box_utils.py
+-rw-r--r--   0        0        0     8510 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/gym/hypergrid.py
+-rw-r--r--   0        0        0     7484 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/modules.py
+-rw-r--r--   0        0        0     1781 2023-08-02 13:35:46.375774 torchgfn-1.0.0/src/gfn/preprocessors.py
+-rw-r--r--   0        0        0     6204 2023-08-02 13:35:46.375774 torchgfn-1.0.0/src/gfn/samplers.py
+-rw-r--r--   0        0        0    15400 2023-08-03 03:55:19.307966 torchgfn-1.0.0/src/gfn/states.py
+-rw-r--r--   0        0        0       40 2023-08-02 13:35:46.375774 torchgfn-1.0.0/src/gfn/utils/__init__.py
+-rw-r--r--   0        0        0     2760 2023-08-02 13:35:46.375774 torchgfn-1.0.0/src/gfn/utils/common.py
+-rw-r--r--   0        0        0     1185 2023-08-02 13:35:46.375774 torchgfn-1.0.0/src/gfn/utils/distributions.py
+-rw-r--r--   0        0        0     4857 2023-08-02 13:35:46.375774 torchgfn-1.0.0/src/gfn/utils/modules.py
+-rw-r--r--   0        0        0    14987 1970-01-01 00:00:00.000000 torchgfn-1.0.0/PKG-INFO
```

### Comparing `torchgfn-0.2/README.md` & `torchgfn-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <p align="center">
     <a>
 	    <img src='https://img.shields.io/badge/python-3.10%2B-blueviolet' alt='Python' />
 	</a>
-	<a href='https://gfn.readthedocs.io/en/latest/?badge=latest'>
-    	<img src='https://readthedocs.org/projects/gfn/badge/?version=latest' alt='Documentation Status' />
+	<a href='https://torchgfn.readthedocs.io/en/latest/?badge=latest'>
+    	<img src='https://readthedocs.org/projects/torchgfn/badge/?version=latest' alt='Documentation Status' />
 	</a>
     <a>
 	    <img src='https://img.shields.io/badge/code%20style-black-black' />
 	</a>
 </p>
 
 </p>
 <p align="center">
-  <a href="https://gfn.readthedocs.io/en/latest/">Documentation</a> ~ <a href="https://github.com/saleml/gfn">Code</a>
+  <a href="https://torchgfn.readthedocs.io/en/latest/">Documentation</a> ~ <a href="https://github.com/saleml/torchgfn">Code</a> ~ <a href="https://arxiv.org/abs/2305.14594">Paper</a>
 </p>
 
-# gfn: a Python package for GFlowNets
+# torchgfn: a Python package for GFlowNets
 
+<p align="center"> Please cite <a href="https://arxiv.org/abs/2305.14594">this paper</a> if you are using the library for your research </p>
 
-
-## Installing the packages
+## Installing the package
 
 The codebase requires python >= 3.10
 
 To install the latest stable version:
 
 ```bash
 pip install torchgfn
@@ -34,174 +34,169 @@
 ```bash
 pip install torchgfn[scripts]
 ```
 
 To install the cutting edge version (from the `main` branch):
 
 ```bash
-git clone https://github.com/saleml/gfn.git
-conda create -n gfn python=3.11
+git clone https://github.com/saleml/torchgfn.git
+conda create -n gfn python=3.10
 conda activate gfn
-cd gfn
+cd torchgfn
 pip install .
 ```
 
 
 ## About this repo
 
-This repo serves the purpose of fast prototyping [GFlowNet](https://arxiv.org/abs/2111.09266) related algorithms. It decouples the environment definition, the sampling process, and the parametrization used for the GFN loss.
+This repo serves the purpose of fast prototyping [GFlowNet](https://arxiv.org/abs/2111.09266) related algorithms. It decouples the environment definition, the sampling process, and the parametrization of the function approximators used to calculate the GFN loss.
 
-An example script is provided [here](https://github.com/saleml/gfn/blob/master/scripts/train.py). To run the code, use one of the following:
+Example scripts and notebooks are provided [here](https://github.com/saleml/torchgfn/tree/master/tutorials/).
 
-```bash
-python train.py --env hypergrid --env.ndim 4 --env.height 8 --n_iterations 100000 --loss trajectory-balance
-python train.py --env discrete-ebm --env.ndim 4 --env.alpha 0.5 --n_iterations 10000 --batch_size 64 --sampler.temperature 2.
-python train.py --env hypergrid --env.ndim 2 --env.height 64 --n_iterations 100000 --loss detailed-balance --logit_PB.module_name Uniform --optim adam --optim.lr 1e-3 --batch_size 64
-python train.py --env hypergrid --env.ndim 4 --env.height 8 --env.R0 0.01 --loss flowmatching --optim adam --optim.lr 1e-4
-```
 
-### Example, in a few lines
+### Standalone example
 
-(⬇️ This example require the [`tqdm`](https://github.com/tqdm/tqdm) package to run. `pip install tqdm` or install all extra requirements with `pip install .[scripts]`)
+This example, which shows how to use the library for a simple discrete environment, requires [`tqdm`](https://github.com/tqdm/tqdm) package to run. Use `pip install tqdm` or install all extra requirements with `pip install .[scripts]` or `pip install torchgfn[scripts]`.
 
 ```python
 import torch
 from tqdm import tqdm
 
-from gfn import LogitPBEstimator, LogitPFEstimator, LogZEstimator
-from gfn.envs import HyperGrid
-from gfn.losses import TBParametrization, TrajectoryBalance
-from gfn.samplers import DiscreteActionsSampler, TrajectoriesSampler
+from gfn.gflownet import TBGFlowNet
+from gfn.gym import HyperGrid
+from gfn.modules import DiscretePolicyEstimator
+from gfn.samplers import Sampler
+from gfn.utils import NeuralNet
 
 if __name__ == "__main__":
 
     env = HyperGrid(ndim=4, height=8, R0=0.01)  # Grid of size 8x8x8x8
 
-    logit_PF = LogitPFEstimator(env=env, module_name="NeuralNet")
-    logit_PB = LogitPBEstimator(
-        env=env,
-        module_name="NeuralNet",
-        torso=logit_PF.module.torso,  # To share parameters between PF and PB
+    module_PF = NeuralNet(
+        input_dim=env.preprocessor.output_dim,
+        output_dim=env.n_actions
     )
-    logZ = LogZEstimator(torch.tensor(0.0))
+    module_PB = NeuralNet(
+        input_dim=env.preprocessor.output_dim,
+        output_dim=env.n_actions - 1,
+        torso=module_PF.torso
+    )
+
+    pf_estimator = DiscretePolicyEstimator(env, module_PF, forward=True)
+    pb_estimator = DiscretePolicyEstimator(env, module_PB, forward=False)
 
-    parametrization = TBParametrization(logit_PF, logit_PB, logZ)
+    gfn = TBGFlowNet(init_logZ=0., pf=pf_estimator, pb=pb_estimator)
 
-    actions_sampler = DiscreteActionsSampler(estimator=logit_PF)
-    trajectories_sampler = TrajectoriesSampler(env=env, actions_sampler=actions_sampler)
+    sampler = Sampler(estimator=pf_estimator))
 
-    loss_fn = TrajectoryBalance(parametrization=parametrization)
+    # Policy parameters have their own LR.
+    non_logz_params = [v for k, v in dict(gfn.named_parameters()).items() if k != "logZ"]
+    optimizer = torch.optim.Adam(non_logz_params, lr=1e-3)
 
-    params = [
-        {
-            "params": [
-                val for key, val in parametrization.parameters.items() if "logZ" not in key
-            ],
-            "lr": 0.001,
-        },
-        {"params": [val for key, val in parametrization.parameters.items() if "logZ" in key], "lr": 0.1},
-    ]
-    optimizer = torch.optim.Adam(params)
+    # Log Z gets dedicated learning rate (typically higher).
+    logz_params = [dict(gfn.named_parameters())["logZ"]]
+    optimizer.add_param_group({"params": logz_params, "lr": 1e-2})
 
     for i in (pbar := tqdm(range(1000))):
-        trajectories = trajectories_sampler.sample(n_trajectories=16)
+        trajectories = sampler.sample_trajectories(n_trajectories=16)
         optimizer.zero_grad()
-        loss = loss_fn(trajectories)
+        loss = gfn.loss(trajectories)
         loss.backward()
         optimizer.step()
         if i % 25 == 0:
             pbar.set_postfix({"loss": loss.item()})
-
 ```
 
 ## Contributing
 
 Before the first commit:
 
 ```bash
-pip install .[dev]
+pip install -e .[dev,scripts]
 pre-commit install
 pre-commit run --all-files
 ```
 
 Run `pre-commit` after staging, and before committing. Make sure all the tests pass (By running `pytest`).
 The codebase uses `black` formatter.
 
 To make the docs locally:
+
 ```bash
 cd docs
 make html
 open build/html/index.html
 ```
 
 ## Details about the codebase
 
 ### Defining an environment
 
-A pointed DAG environment (or GFN environment, or environment for short) is a representation for the pointed DAG. The abstract class [Env](https://github.com/saleml/gfn/blob/master/src/gfn/envs/env.py) specifies the requirements for a valid environment definition. To obtain such a representation, the environment needs to specify the following attributes, properties, or methods:
+See [here](https://github.com/saleml/torchgfn/tree/master/tutorials/ENV.md)
+
+### States
+
+States are the primitive building blocks for GFlowNet objects such as transitions and trajectories, on which losses operate.
 
-- The `action_space`. Which should be a `gymnasium.spaces.Discrete` object for discrete environments. The last action should correspond to the exit action.
-- The initial state `s_0`, as a `torch.Tensor` of arbitrary dimension.
-- (Optional) The sink state `s_f`, as a `torch.Tensor` of the same shape as `s_0`, used to represent complete trajectories only (within a batch of trajectories of different lengths), and never processed by any model. If not specified, it is set to `torch.full_like(s_0, -float('inf'))`.
-- The method `make_States_class` that creates a subclass of [States](https://github.com/saleml/gfn/blob/master/src/gfn/containers/states.py). The instances of the resulting class should represent a batch of states of arbitrary shape, which is useful to define a trajectory, or a batch of trajectories. `s_0` and `s_f`, along with a tuple called `state_shape` should be defined as class variables, and the subclass (of `States`) should implement masking methods, that specify which actions are possible, in a discrete environment.
-- The methods `maskless_step` and `maskless_backward_step` that specify how an action changes a state (going forward and backward). These functions do not need to handle masking, checking whether actions are allowed, checking whether a state is the sink state, etc... These checks are handled in `Env.step` and `Env.backward_step`
-- The `log_reward` function that assigns a nonnegative reward to every terminating state (i.e. state with all $s_f$ as a child in the DAG). If `log_reward` is not implemented, `reward` needs to be.
+An abstract `States` class is provided. But for each environment, a `States` subclass is needed. A `States` object
+is a collection of multiple states (nodes of the DAG). A tensor representation of the states is required for batching. If a state is represented with a tensor of shape `(*state_shape)`, a batch of states is represented with a `States` object, with the attribute `tensor` of shape `(*batch_shape, *state_shape)`. Other
+representations are possible (e.g. a state as a string, a `numpy` array, a graph, etc...), but these representations cannot be batched, unless the user specifies a function that transforms these raw states to tensors.
 
-If the states (as represented in the `States` class) need to be transformed to another format before being processed (by neural networks for example), then the environment should define a `preprocessor` attribute, which should be an instance of the [base preprocessor class](https://github.com/saleml/gfn/blob/master/src/gfn/envs/preprocessors/base.py). If no preprocessor is defined, the states are used as is (actually transformed using  [`IdentityPreprocessor`](https://github.com/saleml/gfn/blob/master/src/gfn/envs/preprocessors/base.py), which transforms the state tensors to `FloatTensor`s). Implementing your own preprocessor requires defining the `preprocess` function, and the `output_shape` attribute, which is a tuple representing the shape of *one* preprocessed state.
+The `batch_shape` attribute is required to keep track of the batch dimension. A trajectory can be represented by a States object with `batch_shape = (n_states,)`. Multiple trajectories can be represented by a States object with `batch_shape = (n_states, n_trajectories)`.
 
-Optionally, you can define a static `get_states_indices` method that assigns a unique integer number to each state if the environment allows it, and a `n_states` property that returns an integer representing the number of states (excluding $s_f$) in the environment. `get_terminating_states_indices` can also be implemented and serves the purpose of uniquely identifying terminating states of the environment.
+Because multiple trajectories can have different lengths, batching requires appending a dummy tensor to trajectories that are shorter than the longest trajectory. The dummy state is the $s_f$ attribute of the environment (e.g. `[-1, ..., -1]`, or `[-inf, ..., -inf]`, etc...). Which is never processed, and is used to pad the batch of states only.
 
-For more details, take a look at [HyperGrid](https://github.com/saleml/gfn/blob/master/src/gfn/envs/hypergrid.py), an environment where all states are terminating states, or at [DiscreteEBM](https://github.com/saleml/gfn/blob/master/src/gfn/envs/discrete_ebm.py), where all trajectories are of the same length but only some states are terminating.
+For discrete environments, the action set is represented with the set $\{0, \dots, n_{actions} - 1\}$, where the $(n_{actions})$-th action always corresponds to the exit or terminate action, i.e. that results in a transition of the type $s \rightarrow s_f$, but not all actions are possible at all states. Each `States` object is endowed with two extra attributes: `forward_masks` and `backward_masks`, representing which actions are allowed at each state and which actions could have led to each state, respectively. Such states are instances of the `DiscreteStates` abstract subclass of `States`. The `forward_masks` tensor is of shape `(*batch_shape, n_{actions})`, and `backward_masks` is of shape `(*batch_shape, n_{actions} - 1)`. Each subclass of `DiscreteStates` needs to implement the `update_masks` function, that uses the environment's logic to define the two tensors.
 
-### Other containers
+### Actions
+Actions should be though of as internal actions of an agent building a compositional object. They correspond to transitions $s \rightarrow s'$. An abstract `Actions` class is provided. It is automatically subclassed for discrete environments, but needs to be manually subclassed otherwise.
 
-Besides the `States` class, other containers of states are available:
+Similar to `States` objects, each action is a tensor of shape `(*batch_shape, *action_shape)`. For discrete environments for instances, `action_shape = (1,)`, representing an integer between $0$ and $n_{actions} - 1$.
 
-- [Transitions](https://github.com/saleml/gfn/blob/master/src/gfn/containers/transitions.py), representing a batch of transitions $s \rightarrow s'$.
-- [Trajectories](https://github.com/saleml/gfn/blob/master/src/gfn/containers/trajectories.py), representing a batch of complete trajectories $\tau = s_0 \rightarrow s_1 \rightarrow \dots \rightarrow s_n \rightarrow s_f$.
+Additionally, each subclass needs to define two more class variable tensors:
+- `dummy_action`: A tensor that is padded to sequences of actions in the shorter trajectories of a batch of trajectories. It is `[-1]` for discrete environments.
+- `exit_action`: A tensor that corresponds to the termination action. It is `[n_{actions} - 1]` fo discrete environments.
 
-These containers can either be instantiated using a `States` object, or can be initialized as empty containers that can be populated on the fly, allowing the usage of [ReplayBuffer](https://github.com/saleml/gfn/blob/master/src/gfn/containers/replay_buffer.py)s.
+### Containers
 
-They inherit from the base `Container` [class](https://github.com/saleml/gfn/blob/master/src/gfn/containers/base.py), indicating some helpful methods.
+Containers are collections of `States`, along with other information, such as reward values, or densities $p(s' \mid s)$. Two containers are available:
 
-In most cases, one needs to sample complete trajectories. From a batch of trajectories, a batch of states and batch of transitions can be defined using `Trajectories.to_transitions()` and `Trajectories.to_states()`. These exclude meaningless transitions and states that were added to the batch of trajectories to allow for efficient batching.
+- [Transitions](https://github.com/saleml/torchgfn/tree/master/src/gfn/containers/transitions.py), representing a batch of transitions $s \rightarrow s'$.
+- [Trajectories](https://github.com/saleml/torchgfn/tree/master/src/gfn/containers/trajectories.py), representing a batch of complete trajectories $\tau = s_0 \rightarrow s_1 \rightarrow \dots \rightarrow s_n \rightarrow s_f$.
 
-### Estimators and Modules
+These containers can either be instantiated using a `States` object, or can be initialized as empty containers that can be populated on the fly, allowing the usage of the[ReplayBuffer](https://github.com/saleml/torchgfn/tree/master/src/gfn/containers/replay_buffer.py) class.
 
-Training GFlowNets requires one or multiple estimators. As of now, only discrete environments are handled. All estimators are subclasses of [FunctionEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py), implementing a `__call__` function that takes as input a batch of [States](https://github.com/saleml/gfn/blob/master/src/gfn/containers/states.py).
+They inherit from the base `Container` [class](https://github.com/saleml/torchgfn/tree/master/src/gfn/containers/base.py), indicating some helpful methods.
 
-- [LogEdgeFlowEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, n_actions)` tensor representing $\log F(s \rightarrow s')$, including when $s' = s_f$.
-- [LogStateFlowEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, 1)` tensor representing $\log F(s)$. When used with `forward_looking=True`, $\log F(s)$ is parametrized as the sum of a function approximator and $\log R(s)$ - which is only possible for environments where all states are terminating.
-- [LogitPFEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, n_actions)` tensor representing $logit(s' \mid s)$, such that $P_F(s' \mid s) = softmax_{s'}\ logit(s' \mid s)$, including when $s' = s_f$.
-- [LogitPBEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, n_actions - 1)` tensor representing $logit(s' \mid s)$, such that $P_B(s' \mid s) = softmax_{s'}\ logit(s' \mid s)$.
+In most cases, one needs to sample complete trajectories. From a batch of trajectories, a batch of states and batch of transitions can be defined using `Trajectories.to_transitions()` and `Trajectories.to_states()`. These exclude meaningless transitions and dummy states that were added to the batch of trajectories to allow for efficient batching.
 
-Defining an estimator requires the environment, and a [module](https://github.com/saleml/gfn/blob/master/src/gfn/modules.py) instance. Modules inherit from the [GFNModule](https://github.com/saleml/gfn/blob/master/src/gfn/modules.py) class, which can be seen as an extension of `torch.nn.Module`. Alternatively, a module is created by providing which module type to use (e.g. "NeuralNet" or "Uniform" or "Zero"). A Basic MLP is provided as the [NeuralNet](https://github.com/saleml/gfn/blob/master/src/gfn/modules.py) class, but any function approximator should be possible.
+### Modules
 
-Said differently, a `States` object is first transformed via the environment's preprocessor to a `(*batch_shape, *output_shape)` float tensor. The preprocessor's output shape should match the module input shape (if any). The preprocessed states are then passed as inputs to the module, returning the desired output (either flows or probabilities over children in the DAG).
+Training GFlowNets requires one or multiple estimators, called `GFNModule`s, which is an abstract subclass of `torch.nn.Module`. In addition to the usual `forward` function, `GFNModule`s need to implement a `required_output_dim` attribute, to ensure that the outputs have the required dimension for the task at hand; and some (but not all) need to implement a `to_probability_distribution` function. They take the environment `env` as an input at initialization.
+- `DiscretePolicyEstimator` is a `GFNModule` that defines the policies $P_F(. \mid s)$ and $P_B(. \mid s)$ for discrete environments. When `backward=False`, the required output dimension is `n = env.n_actions`, and when `backward=True`, it is `n = env.n_actions - 1`. These `n` numbers represent the logits of a Categorical distribution. Additionally, they include exploration parameters, in order to define a tempered version of $P_F$, or a mixture of $P_F$ with a uniform distribution. Naturally, before defining the Categorical distributions, forbidden actions (that are encoded in the `DiscreteStates`' masks attributes), are given 0 probability by setting the corresponding logit to $-\infty$.
+- `ScalarModule` is a simple module with required output dimension 1. It is useful to define log-state flows $\log F(s)$.
 
-Each module has a `named_parameters` functions that returns a dictionary of the learnable parameters. This attribute is transferred to the corresponding estimator.
+For non-discrete environments, the user needs to specify their own policies $P_F$ and $P_B$. The module, taking as input a batch of states (as a `States`) object, should return the batched parameters of a `torch.Distribution`. The distribution depends on the environment. The `to_probability_distribution` function handles the conversion of the parameter outputs to an actual batched `Distribution` object, that implements at least the `sample` and `log_prob` functions. An example is provided [here](https://github.com/saleml/torchgfn/tree/master/src/gfn/gym/helpers/box_utils.py), for a square environment in which the forward policy has support either on a quarter disk, or on an arc-circle, such that the angle, and the radius (for the quarter disk part) are scaled samples from a mixture of Beta distributions. The provided example shows an intricate scenario, and it is not expected that user defined environment need this much level of details.
 
-Additionally, a [LogZEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py) is provided, which is a container for a scalar tensor representing $\log Z$, the log-partition function, useful for the Trajectory Balance loss for example. This estimator also has a `named_parameters` function.
+In all `GFNModule`s, note that the input of the `forward` function is a `States` object. Meaning that they first need to be transformed to tensors. However, `states.tensor` does not necessarily include the structure that a neural network can used to generalize. It is common in these scenarios to have a function that transforms these raw tensor states to ones where the structure is clearer, via a `Preprocessor` object, that is part of the environment. More on this [here](https://github.com/saleml/torchgfn/tree/master/tutorials/ENV.md). The default preprocessor of an environment is the identity preprocessor. The `forward` pass thus first calls the `preprocessor` attribute of the environment on `States`, before performing any transformation.
+
+For discrete environments, tabular modules are provided, where a lookup table is used instead of a neural network. Additionally, a `UniformPB` module is provided, implementing a uniform backward policy.
 
 ### Samplers
 
-An [ActionsSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/actions_samplers.py) object defines how actions are sampled at each state of the DAG. As of now, only [DiscreteActionsSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/actions_samplers.py)s are implemented. The require an estimator (of $P_F$, $P_B$, or edge flows) defining the action probabilities. These estimators can contain any type of modules (including random action sampling for example). A [BackwardDiscreteActionsSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/actions_samplers.py) class is provided to sample parents of a state, which is helpful to sample trajectories starting from their last states.
+A [Sampler](https://github.com/saleml/torchgfn/tree/master/src/gfn/samplers.py) object defines how actions are sampled (`sample_actions()`) at each state, and trajectories  (`sample_trajectories()`), which can sample a batch of trajectories starting from a given set of initial states or starting from $s_0$. It requires a `GFNModule` that implements the `to_probability_distribution` function.
 
-They are at the core of [TrajectoriesSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/trajectories_sampler.py)s, which implements the `sample_trajectories` method, that sample a batch of trajectories starting from a given set of initial states or starting from $s_0$.
 
 ### Losses
 
-GFlowNets can be trained with different losses, each of which requires a different parametrization. A parametrization is a dataclass, which can be seen as a container of different estimators. Each parametrization defines a distribution over trajectories, via the `parametrization.Pi` method, and a distribution over terminating states, via the `parametrization.P_T` method. Both distributions should be instances of the classes defined [here](https://github.com/saleml/gfn/blob/master/src/gfn/distributions.py).
-
-The base classes for losses and parametrizations are provided [here](https://github.com/saleml/gfn/blob/master/src/gfn/losses/base.py).
+GFlowNets can be trained with different losses, each of which requires a different parametrization, which we call in this library a `GFlowNet`. A `GFlowNet` is a `GFNModule` that includes one or multiple `GFNModules`, at least one of which implements a `to_probability_distribution` function. They also need to implement a `loss` function, that takes as input either states, transitions, or trajectories, depending on the loss.
 
 Currently, the implemented losses are:
 
 - Flow Matching
-- Detailed Balance
+- Detailed Balance (and it's modified variant).
 - Trajectory Balance
-- Sub-Trajectory Balance. By default, each sub-trajectory is weighted geometrically (within the trajectory) depending on its length. This corresponds to the strategy defined [here](https://www.semanticscholar.org/reader/f2c32fe3f7f3e2e9d36d833e32ec55fc93f900f5). Other strategies exist and are implemented [here](https://github.com/saleml/gfn/blob/master/src/gfn/losses/sub_trajectory_balance.py).
+- Sub-Trajectory Balance. By default, each sub-trajectory is weighted geometrically (within the trajectory) depending on its length. This corresponds to the strategy defined [here](https://www.semanticscholar.org/reader/f2c32fe3f7f3e2e9d36d833e32ec55fc93f900f5). Other strategies exist and are implemented [here](https://github.com/saleml/torchgfn/tree/master/src/gfn/losses/sub_trajectory_balance.py).
 - Log Partition Variance loss. Introduced [here](https://arxiv.org/abs/2302.05446)
 
-### Solving for the flows using Dynamic Programming
-
-A simple script that propagates trajectories rewards through the DAG to define edge flows in a deterministic way (by visiting each edge once only) is provided [here](https://github.com/saleml/gfn/blob/master/scripts/dynamic_programming.py). Do not use the script on large environments !
+# Scripts
+Example scripts are provided [here](https://github.com/saleml/torchgfn/tree/master/tutorials/examples/). They can be used to reproduce published results in the HyperGrid environment, and the Box environment.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `torchgfn-0.2/pyproject.toml` & `torchgfn-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,92 @@
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core>=1.0.8"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "torchgfn"
 packages = [{include = "gfn", from = "src"}]
-version = "0.2"
+version = "1.0.0"
 description = "A torch implementation of GFlowNets"
 authors = ["Salem Lahou <salemlahlou9@gmail.com>", "Joseph Viviano <joseph@viviano.ca>", "Victor Schmidt <vsch@pm.me>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-# main deps
-python = "^3.10"
+# core dependencies.
 einops = ">=0.6.1"
-gymnasium = ">=0.28.1"
 numpy = ">=1.21.2"
+python = "^3.10"
 torch = ">=1.9.0"
 torchtyping = ">=0.1.4"
-# dev deps
+
+# dev dependencies.
+black = { version = "22.3.0", optional = true }
+gitmopy = { version = "*", optional = true }
+myst-parser = { version = "*", optional = true }
 pre-commit = { version = "*", optional = true }
 pytest = { version = "*", optional = true }
 renku-sphinx-theme = { version = "*", optional = true }
-sphinx_rtd_theme = { version = "*", optional = true }
+sphinx = { version = "*", optional = true }
 sphinx-autoapi = { version = "*", optional = true }
 sphinx-math-dollar = { version = "*", optional = true }
-sphinx = { version = "*", optional = true }
+sphinx_rtd_theme = { version = "*", optional = true }
 tox = { version = "*", optional = true }
-black = { version = "22.3.0", optional = true }
-myst-parser = { version = "*", optional = true }
-# scripts deps
+
+# scripts dependencies.
 tqdm = { version = "*", optional = true }
 wandb = { version = "*", optional = true }
-simple-parsing = { version = "0.0.20", optional = true }
+scikit-learn = {version = "*", optional = true }
+scipy = { version = "*", optional = true }
 
 [tool.poetry.extras]
 dev = [
+    "black",
+    "gitmopy",
+    "myst-parser",
+    "pre-commit",
+    "pytest",
+    "renku-sphinx-theme",
+    "sphinx",
+    "sphinx-autoapi",
+    "sphinx-math-dollar",
+    "sphinx_rtd_theme",
+    "tox"
+]
+
+scripts = ["tqdm", "wandb", "scikit-learn", "scipy"]
+
+all = [
     "pre-commit",
     "pytest",
     "renku-sphinx-theme",
     "sphinx_rtd_theme",
     "sphinx-autoapi",
     "sphinx-math-dollar",
     "sphinx",
     "tox",
     "black",
-    "myst-parser"
+    "myst-parser",
+    "tqdm",
+    "wandb",
+    "scikit-learn",
+    "scipy"
 ]
-scripts = ["tqdm", "wandb", "simple-parsing"]
-all = ["pre-commit", "pytest", "renku-sphinx-theme", "sphinx_rtd_theme", "sphinx-autoapi", "sphinx-math-dollar", "sphinx", "tox", "black", "myst-parser", "tqdm", "wandb", "simple-parsing"]
 
 [project.urls]
 "Homepage" = "https://gfn.readthedocs.io/en/latest/"
 "Bug Tracker" = "https://github.com/saleml/gfn/issues"
 
 
-# TODO: Could use for examples? Or something else?
-# [project.scripts]
-# gfn_example = "gfn.examples:main"
 
 [tool.black]
 py36 = true
 include = '\.pyi?$'
 exclude = '''/(\.git|\.hg|\.mypy_cache|\.tox|\.venv|build)/g'''
 
 [tool.tox]
@@ -111,16 +129,14 @@
 reportPrivateUsage = "warning"
 reportUntypedFunctionDecorator = "none"
 reportMissingTypeStubs = false
 reportUnboundVariable = "warning"
 reportGeneralTypeIssues = "none"
 
 [tool.pytest.ini_options]
-
-
 # Black-compatibility enforced.
 [tool.isort]
 line_length = 89
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
```

### Comparing `torchgfn-0.2/src/gfn/containers/replay_buffer.py` & `torchgfn-1.0.0/src/gfn/containers/replay_buffer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,72 @@
 from __future__ import annotations
 
 import os
 from typing import TYPE_CHECKING, Literal
 
-from gfn.containers.states import States
 from gfn.containers.trajectories import Trajectories
 from gfn.containers.transitions import Transitions
-from gfn.losses.base import (
-    EdgeDecomposableLoss,
-    Loss,
-    StateDecomposableLoss,
-    TrajectoryDecomposableLoss,
-)
 
 if TYPE_CHECKING:
-    from gfn.envs import Env
+    from gfn.env import Env
+    from gfn.states import States
 
 
 class ReplayBuffer:
+    """A replay buffer of trajectories or transitions.
+
+    Attributes:
+        env: the Environment instance.
+        loss_fn: the Loss instance
+        capacity: the size of the buffer.
+        training_objects: the buffer of objects used for training.
+        terminating_states: a States class representation of $s_f$.
+        objects_type: the type of buffer (transitions, trajectories, or states).
+    """
+
     def __init__(
         self,
         env: Env,
-        loss_fn: Loss | None = None,
-        objects_type: Literal["transitions", "trajectories", "states"] | None = None,
+        objects_type: Literal["transitions", "trajectories", "states"],
         capacity: int = 1000,
     ):
+        """Instantiates a replay buffer.
+        Args:
+            env: the Environment instance.
+            loss_fn: the Loss instance.
+            capacity: the size of the buffer.
+            objects_type: the type of buffer (transitions, trajectories, or states).
+        """
         self.env = env
         self.capacity = capacity
         self.terminating_states = None
-        if objects_type == "trajectories" or isinstance(
-            loss_fn, TrajectoryDecomposableLoss
-        ):
+        if objects_type == "trajectories":
             self.training_objects = Trajectories(env)
             self.objects_type = "trajectories"
-        elif objects_type == "transitions" or isinstance(loss_fn, EdgeDecomposableLoss):
+        elif objects_type == "transitions":
             self.training_objects = Transitions(env)
             self.objects_type = "transitions"
-        elif objects_type == "states" or isinstance(loss_fn, StateDecomposableLoss):
+        elif objects_type == "states":
             self.training_objects = env.States.from_batch_shape((0,))
             self.terminating_states = env.States.from_batch_shape((0,))
             self.objects_type = "states"
         else:
-            raise ValueError(
-                f"Unknown objects_type: {objects_type} and loss_fn: {loss_fn}"
-            )
+            raise ValueError(f"Unknown objects_type: {objects_type}")
 
         self._is_full = False
         self._index = 0
 
     def __repr__(self):
         return f"ReplayBuffer(capacity={self.capacity}, containing {len(self)} {self.objects_type})"
 
     def __len__(self):
         return self.capacity if self._is_full else self._index
 
     def add(self, training_objects: Transitions | Trajectories | tuple[States]):
+        """Adds a training object to the buffer."""
         terminating_states = None
         if isinstance(training_objects, tuple):
             assert self.objects_type == "states" and self.terminating_states is not None
             training_objects, terminating_states = training_objects
 
         to_add = len(training_objects)
 
@@ -70,24 +78,27 @@
 
         if self.terminating_states is not None:
             assert terminating_states is not None
             self.terminating_states.extend(terminating_states)
             self.terminating_states = self.terminating_states[-self.capacity :]
 
     def sample(self, n_trajectories: int) -> Transitions | Trajectories | tuple[States]:
+        """Samples `n_trajectories` training objects from the buffer."""
         if self.terminating_states is not None:
             return (
                 self.training_objects.sample(n_trajectories),
                 self.terminating_states.sample(n_trajectories),
             )
         return self.training_objects.sample(n_trajectories)
 
     def save(self, directory: str):
+        """Saves the buffer to disk."""
         self.training_objects.save(os.path.join(directory, "training_objects"))
         if self.terminating_states is not None:
             self.terminating_states.save(os.path.join(directory, "terminating_states"))
 
     def load(self, directory: str):
+        """Loads the buffer from disk."""
         self.training_objects.load(os.path.join(directory, "training_objects"))
         self._index = len(self.training_objects)
         if self.terminating_states is not None:
             self.terminating_states.load(os.path.join(directory, "terminating_states"))
```

### Comparing `torchgfn-0.2/src/gfn/containers/trajectories.py` & `torchgfn-1.0.0/src/gfn/containers/trajectories.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,102 +1,112 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Sequence
 
 if TYPE_CHECKING:
-    from gfn.envs import Env
-    from gfn.containers.states import States
+    from gfn.actions import Actions
+    from gfn.env import Env
+    from gfn.states import States
 
 import torch
-from torchtyping import TensorType
+from torchtyping import TensorType as TT
 
 from gfn.containers.base import Container
 from gfn.containers.transitions import Transitions
 
-# Typing  --- n_transitions is an int
-Tensor2D = TensorType["max_length", "n_trajectories", torch.long]
-FloatTensor2D = TensorType["max_length", "n_trajectories", torch.float]
-Tensor2D2 = TensorType["n_trajectories", "shape"]
-Tensor1D = TensorType["n_trajectories", torch.long]
-FloatTensor1D = TensorType["n_trajectories", torch.float]
-
 
+# TODO: remove env from this class?
 class Trajectories(Container):
+    """Container for complete trajectories (starting in $s_0$ and ending in $s_f$).
+
+    Trajectories are represented as a States object with bi-dimensional batch shape.
+    Actions are represented as an Actions object with bi-dimensional batch shape.
+    The first dimension represents the time step, the second dimension represents
+    the trajectory index. Because different trajectories may have different lengths,
+    shorter trajectories are padded with the tensor representation of the terminal
+    state ($s_f$ or $s_0$ depending on the direction of the trajectory), and
+    actions is appended with dummy actions. The `when_is_done` tensor represents
+    the time step at which each trajectory ends.
+
+    Attributes:
+        env: The environment in which the trajectories are defined.
+        states: The states of the trajectories.
+        actions: The actions of the trajectories.
+        when_is_done: The time step at which each trajectory ends.
+        is_backward: Whether the trajectories are backward or forward.
+        log_rewards: The log_rewards of the trajectories.
+        log_probs: The log probabilities of the trajectories' actions.
+
+    """
+
     def __init__(
         self,
         env: Env,
         states: States | None = None,
-        actions: Tensor2D | None = None,
-        when_is_done: Tensor1D | None = None,
+        actions: Actions | None = None,
+        when_is_done: TT["n_trajectories", torch.long] | None = None,
         is_backward: bool = False,
-        log_rewards: FloatTensor1D | None = None,
-        log_probs: FloatTensor2D | None = None,
+        log_rewards: TT["n_trajectories", torch.float] | None = None,
+        log_probs: TT["max_length", "n_trajectories", torch.float] | None = None,
     ) -> None:
-        """Container for complete trajectories (starting in s_0 and ending in s_f).
-        Trajectories are represented as a States object with bi-dimensional batch shape.
-        The first dimension represents the time step, the second dimension represents the trajectory index.
-        Because different trajectories may have different lengths, shorter trajectories are padded with
-        the tensor representation of the terminal state (s_f or s_0 depending on the direction of the trajectory), and
-        actions is appended with -1's.
-        The actions are represented as a two dimensional tensor with the first dimension representing the time step
-        and the second dimension representing the trajectory index.
-        The when_is_done tensor represents the time step at which each trajectory ends.
-
-
+        """
         Args:
-            env (Env): The environment in which the trajectories are defined.
-            states (States, optional): The states of the trajectories. Defaults to None.
-            actions (Tensor2D, optional): The actions of the trajectories. Defaults to None.
-            when_is_done (Tensor1D, optional): The time step at which each trajectory ends. Defaults to None.
-            is_backward (bool, optional): Whether the trajectories are backward or forward. Defaults to False.
-            log_rewards (FloatTensor1D, optional): The log_rewards of the trajectories. Defaults to None.
-            log_probs (FloatTensor2D, optional): The log probabilities of the trajectories' actions. Defaults to None.
-
-        If states is None, then the states are initialized to an empty States object, that can be populated on the fly.
-        If log_rewards is None, then `env.log_reward` is used to compute the rewards, at each call of self.log_rewards
+            env: The environment in which the trajectories are defined.
+            states: The states of the trajectories. Defaults to None.
+            actions: The actions of the trajectories. Defaults to None.
+            when_is_done: The time step at which each trajectory ends. Defaults to None.
+            is_backward: Whether the trajectories are backward or forward. Defaults to False.
+            log_rewards: The log_rewards of the trajectories. Defaults to None.
+            log_probs: The log probabilities of the trajectories' actions. Defaults to None.
+
+        If states is None, then the states are initialized to an empty States object,
+        that can be populated on the fly. If log_rewards is None, then `env.log_reward`
+        is used to compute the rewards, at each call of self.log_rewards
         """
         self.env = env
         self.is_backward = is_backward
         self.states = (
             states
             if states is not None
             else env.States.from_batch_shape(batch_shape=(0, 0))
         )
         assert len(self.states.batch_shape) == 2
         self.actions = (
             actions
             if actions is not None
-            else torch.full(size=(0, 0), fill_value=-1, dtype=torch.long)
+            else env.Actions.make_dummy_actions(batch_shape=(0, 0))
         )
+        assert len(self.actions.batch_shape) == 2
         self.when_is_done = (
             when_is_done
             if when_is_done is not None
             else torch.full(size=(0,), fill_value=-1, dtype=torch.long)
         )
         self._log_rewards = log_rewards
         self.log_probs = (
             log_probs
             if log_probs is not None
             else torch.full(size=(0, 0), fill_value=0, dtype=torch.float)
         )
 
     def __repr__(self) -> str:
-        states = self.states.states_tensor.transpose(0, 1)
+        states = self.states.tensor.transpose(0, 1)
         assert states.ndim == 3
         trajectories_representation = ""
         for traj in states[:10]:
             one_traj_repr = []
             for step in traj:
                 one_traj_repr.append(str(step.numpy()))
                 if step.equal(self.env.s0 if self.is_backward else self.env.sf):
                     break
             trajectories_representation += "-> ".join(one_traj_repr) + "\n"
         return (
             f"Trajectories(n_trajectories={self.n_trajectories}, max_length={self.max_length}, First 10 trajectories:"
-            + f"states=\n{trajectories_representation}, actions=\n{self.actions.transpose(0, 1)[:10].numpy()}, "
+            + f"states=\n{trajectories_representation}"
+            # + f"actions=\n{self.actions.tensor.squeeze().transpose(0, 1)[:10].numpy()}, "
             + f"when_is_done={self.when_is_done[:10].numpy()})"
         )
 
     @property
     def n_trajectories(self) -> int:
         return self.states.batch_shape[1]
 
@@ -104,167 +114,141 @@
         return self.n_trajectories
 
     @property
     def max_length(self) -> int:
         if len(self) == 0:
             return 0
 
-        return self.actions.shape[0]
+        return self.actions.batch_shape[0]
 
     @property
     def last_states(self) -> States:
         return self.states[self.when_is_done - 1, torch.arange(self.n_trajectories)]
 
     @property
-    def log_rewards(self) -> FloatTensor1D | None:
+    def log_rewards(self) -> TT["n_trajectories", torch.float] | None:
         if self._log_rewards is not None:
             assert self._log_rewards.shape == (self.n_trajectories,)
             return self._log_rewards
         if self.is_backward:
             return None
         try:
             return self.env.log_reward(self.last_states)
         except NotImplementedError:
             return torch.log(self.env.reward(self.last_states))
 
     def __getitem__(self, index: int | Sequence[int]) -> Trajectories:
-        "Returns a subset of the `n_trajectories` trajectories."
+        """Returns a subset of the `n_trajectories` trajectories."""
         if isinstance(index, int):
             index = [index]
         when_is_done = self.when_is_done[index]
         new_max_length = when_is_done.max().item() if len(when_is_done) > 0 else 0
         states = self.states[:, index]
         actions = self.actions[:, index]
-        log_probs = self.log_probs[:, index]
         states = states[: 1 + new_max_length]
         actions = actions[:new_max_length]
-        log_probs = log_probs[:new_max_length]
+        if self.log_probs.shape != (0, 0):
+            log_probs = self.log_probs[:, index]
+            log_probs = log_probs[:new_max_length]
+        else:
+            log_probs = self.log_probs
         log_rewards = (
             self._log_rewards[index] if self._log_rewards is not None else None
         )
 
         return Trajectories(
             env=self.env,
             states=states,
             actions=actions,
             when_is_done=when_is_done,
             is_backward=self.is_backward,
             log_rewards=log_rewards,
             log_probs=log_probs,
         )
 
+    @staticmethod
+    def extend_log_probs(
+        log_probs: TT["max_length", "n_trajectories", torch.float], new_max_length: int
+    ) -> TT["max_max_length", "n_trajectories", torch.float]:
+        """Extend the log_probs matrix by adding 0 until the required length is reached."""
+        if log_probs.shape[0] >= new_max_length:
+            return log_probs
+        else:
+            return torch.cat(
+                (
+                    log_probs,
+                    torch.full(
+                        size=(
+                            new_max_length - log_probs.shape[0],
+                            log_probs.shape[1],
+                        ),
+                        fill_value=0,
+                        dtype=torch.float,
+                        device=log_probs.device,
+                    ),
+                ),
+                dim=0,
+            )
+
     def extend(self, other: Trajectories) -> None:
-        """Extend the trajectories with another set of trajectories."""
-        self.extend_actions(required_first_dim=max(self.max_length, other.max_length))
-        other.extend_actions(required_first_dim=max(self.max_length, other.max_length))
+        """Extend the trajectories with another set of trajectories.
+
+        Extends along all attributes in turn (actions, states, when_is_done, log_probs,
+        log_rewards).
+
+        Args:
+            other: an external set of Trajectories.
+        """
 
+        self.actions.extend(other.actions)
         self.states.extend(other.states)
-        self.actions = torch.cat((self.actions, other.actions), dim=1)
         self.when_is_done = torch.cat((self.when_is_done, other.when_is_done), dim=0)
+
+        # For log_probs, we first need to make the first dimensions of self.log_probs and other.log_probs equal
+        # (i.e. the number of steps in the trajectories), and then concatenate them
+        new_max_length = max(self.log_probs.shape[0], other.log_probs.shape[0])
+        self.log_probs = self.extend_log_probs(self.log_probs, new_max_length)
+        other.log_probs = self.extend_log_probs(other.log_probs, new_max_length)
+
         self.log_probs = torch.cat((self.log_probs, other.log_probs), dim=1)
 
         if self._log_rewards is not None and other._log_rewards is not None:
             self._log_rewards = torch.cat(
                 (self._log_rewards, other._log_rewards), dim=0
             )
         else:
             self._log_rewards = None
 
-    def extend_actions(self, required_first_dim: int) -> None:
-        """Extends the actions and log_probs along the first dimension by by adding -1s as necessary.
-        This is useful for extending trajectories of different lengths."""
-        if self.max_length >= required_first_dim:
-            return
-        self.actions = torch.cat(
-            (
-                self.actions,
-                torch.full(
-                    size=(
-                        required_first_dim - self.actions.shape[0],
-                        self.n_trajectories,
-                    ),
-                    fill_value=-1,
-                    dtype=torch.long,
-                ),
-            ),
-            dim=0,
-        )
-        self.log_probs = torch.cat(
-            (
-                self.log_probs,
-                torch.full(
-                    size=(
-                        required_first_dim - self.log_probs.shape[0],
-                        self.n_trajectories,
-                    ),
-                    fill_value=0,
-                    dtype=torch.float,
-                ),
-            ),
-            dim=0,
-        )
-
-    @staticmethod
-    def revert_backward_trajectories(trajectories: Trajectories) -> Trajectories:
-
-        assert trajectories.is_backward
-        new_actions = torch.full_like(trajectories.actions, -1)
-        new_actions = torch.cat(
-            [new_actions, torch.full((1, len(trajectories)), -1)], dim=0
-        )
-        new_states = trajectories.env.sf.repeat(
-            trajectories.when_is_done.max() + 1, len(trajectories), 1
-        )
-        new_when_is_done = trajectories.when_is_done + 1
-        for i in range(len(trajectories)):
-            new_actions[trajectories.when_is_done[i], i] = (
-                trajectories.env.n_actions - 1
-            )
-            new_actions[: trajectories.when_is_done[i], i] = trajectories.actions[
-                : trajectories.when_is_done[i], i
-            ].flip(0)
-            new_states[
-                : trajectories.when_is_done[i] + 1, i
-            ] = trajectories.states.states_tensor[
-                : trajectories.when_is_done[i] + 1, i
-            ].flip(
-                0
-            )
-        new_states = trajectories.env.States(new_states)
-        return Trajectories(
-            env=trajectories.env,
-            states=new_states,
-            actions=new_actions,
-            log_probs=trajectories.log_probs,
-            when_is_done=new_when_is_done,
-            is_backward=False,
-        )
-
     def to_transitions(self) -> Transitions:
-        """Returns a `Transitions` object from the trajectories"""
-        states = self.states[:-1][self.actions != -1]
-        next_states = self.states[1:][self.actions != -1]
-        actions = self.actions[self.actions != -1]
+        """Returns a `Transitions` object from the trajectories."""
+        states = self.states[:-1][~self.actions.is_dummy]
+        next_states = self.states[1:][~self.actions.is_dummy]
+        actions = self.actions[~self.actions.is_dummy]
         is_done = (
             next_states.is_sink_state
             if not self.is_backward
             else next_states.is_initial_state
         )
         if self._log_rewards is None:
             log_rewards = None
         else:
-            log_rewards = torch.full_like(actions, fill_value=-1.0, dtype=torch.float)
+            log_rewards = torch.full(
+                actions.batch_shape,
+                fill_value=-float("inf"),
+                dtype=torch.float,
+                device=actions.device,
+            )
             log_rewards[is_done] = torch.cat(
                 [
                     self._log_rewards[self.when_is_done == i]
                     for i in range(self.when_is_done.max() + 1)
                 ],
                 dim=0,
             )
-        log_probs = self.log_probs[self.actions != -1]
+        log_probs = self.log_probs[~self.actions.is_dummy]
         return Transitions(
             env=self.env,
             states=states,
             actions=actions,
             is_done=is_done,
             next_states=next_states,
             is_backward=self.is_backward,
@@ -276,18 +260,20 @@
         """Returns a `States` object from the trajectories, containing all states in the trajectories"""
         states = self.states.flatten()
         return states[~states.is_sink_state]
 
     def to_non_initial_intermediary_and_terminating_states(
         self,
     ) -> tuple[States, States]:
-        """Returns a tuple of `States` objects from the trajectories, containing all non-initial intermediary and all terminating states in the trajectories
+        """Returns all intermediate and terminating `States` from the trajectories.
+
+        This is useful for the flow matching loss, that requires its inputs to be distinguished.
 
-        Returns:
-            Tuple[States, States]: - All the intermediary states in the trajectories that are not s0.
-                                   - All the terminating states in the trajectories that are not s0.
+        Returns: a tuple containing all the intermediary states in the trajectories
+            that are not s0, and all the terminating states in the trajectories that
+            are not s0.
         """
         states = self.states
         intermediary_states = states[~states.is_sink_state & ~states.is_initial_state]
         terminating_states = self.last_states
         terminating_states.log_rewards = self.log_rewards
         return intermediary_states, terminating_states
```

### Comparing `torchgfn-0.2/src/gfn/containers/transitions.py` & `torchgfn-1.0.0/src/gfn/containers/transitions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,85 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Sequence
 
 import torch
-from torchtyping import TensorType
+from torchtyping import TensorType as TT
 
 if TYPE_CHECKING:
-    from gfn.envs import Env
-    from gfn.containers.states import States
+    from gfn.actions import Actions
+    from gfn.env import Env
+    from gfn.states import States
 
 from gfn.containers.base import Container
 
-# Typing  -- n_transitions is either int or Tuple[int]
-LongTensor = TensorType["n_transitions", torch.long]
-BoolTensor = TensorType["n_transitions", torch.bool]
-FloatTensor = TensorType["n_transitions", torch.float]
-PairFloatTensor = TensorType["n_transitions", 2, torch.float]
-
 
 class Transitions(Container):
+    """Container for the transitions.
+
+    Attributes:
+        env: environment.
+        is_backward: Whether the transitions are backward transitions (i.e.
+            `next_states` is the parent of states).
+        states: States object with uni-dimensional `batch_shape`, representing the
+            parents of the transitions.
+        actions: Actions chosen at the parents of each transitions.
+        is_done: Whether the action is the exit action.
+        next_states: States object with uni-dimensional `batch_shape`, representing
+            the children of the transitions.
+        log_probs: The log-probabilities of the actions.
+    """
+
     def __init__(
         self,
         env: Env,
         states: States | None = None,
-        actions: LongTensor | None = None,
-        is_done: BoolTensor | None = None,
+        actions: Actions | None = None,
+        is_done: TT["n_transitions", torch.bool] | None = None,
         next_states: States | None = None,
         is_backward: bool = False,
-        log_rewards: FloatTensor | None = None,
-        log_probs: FloatTensor | None = None,
+        log_rewards: TT["n_transitions", torch.float] | None = None,
+        log_probs: TT["n_transitions", torch.float] | None = None,
     ):
-        """Container for transitions.
+        """Instantiates a container for transitions.
 
-        Args:
-            env (Env): Environment
-            states (States, optional): States object with uni-dimensional batch_shape, representing the parents of the transitions. Defaults to None.
-            actions (LongTensor, optional): Actions chosen at the parents of each transitions. Defaults to None.
-            is_done (BoolTensor, optional): Whether the action is the exit action. Defaults to None.
-            next_states (States, optional): States object with uni-dimensional batch_shape, representing the children of the transitions. Defaults to None.
-            is_backward (bool, optional): Whether the transitions are backward transitions (i.e. next_states is the parent of states). Defaults to False.
-            log_rewards (FloatTensor1D, optional): The log-rewards of the transitions (using a default value like -1 for non-terminating transitions). Defaults to None.
-            log_probs (FloatTensor1D, optional): The log-probabilities of the actions. Defaults to None.
+        When states and next_states are not None, the Transitions is an empty container
+        that can be populated on the go.
 
-        When states and next_states are not None, the Transitions is an empty container that can be populated on the go.
+        Args:
+            env: Environment
+            states: States object with uni-dimensional `batch_shape`, representing the
+                parents of the transitions.
+            actions: Actions chosen at the parents of each transitions.
+            is_done: Whether the action is the exit action.
+            next_states: States object with uni-dimensional `batch_shape`, representing
+                the children of the transitions.
+            is_backward: Whether the transitions are backward transitions (i.e.
+                `next_states` is the parent of states).
+            log_rewards: The log-rewards of the transitions (using a default value like
+                `-float('inf')` for non-terminating transitions).
+            log_probs: The log-probabilities of the actions.
+
+        Raises:
+            AssertionError: If states and next_states do not have matching
+                `batch_shapes`.
         """
         self.env = env
         self.is_backward = is_backward
         self.states = (
             states
             if states is not None
             else env.States.from_batch_shape(batch_shape=(0,))
         )
         assert len(self.states.batch_shape) == 1
+
         self.actions = (
             actions
             if actions is not None
-            else torch.full(size=(0,), fill_value=-1, dtype=torch.long)
+            else env.Actions.make_dummy_actions(batch_shape=(0,))
         )
         self.is_done = (
             is_done
             if is_done is not None
             else torch.full(size=(0,), fill_value=False, dtype=torch.bool)
         )
         self.next_states = (
@@ -67,29 +87,27 @@
             if next_states is not None
             else env.States.from_batch_shape(batch_shape=(0,))
         )
         assert (
             len(self.next_states.batch_shape) == 1
             and self.states.batch_shape == self.next_states.batch_shape
         )
-
         self._log_rewards = log_rewards
-
         self.log_probs = log_probs if log_probs is not None else torch.zeros(0)
 
     @property
     def n_transitions(self) -> int:
         return self.states.batch_shape[0]
 
     def __len__(self) -> int:
         return self.n_transitions
 
     def __repr__(self):
-        states_tensor = self.states.states_tensor
-        next_states_tensor = self.next_states.states_tensor
+        states_tensor = self.states.tensor
+        next_states_tensor = self.next_states.tensor
 
         states_repr = ",\t".join(
             [
                 f"{str(state.numpy())} -> {str(next_state.numpy())}"
                 for state, next_state in zip(states_tensor, next_states_tensor)
             ]
         )
@@ -101,43 +119,49 @@
 
     @property
     def last_states(self) -> States:
         "Get the last states, i.e. terminating states"
         return self.states[self.is_done]
 
     @property
-    def log_rewards(self) -> FloatTensor | None:
+    def log_rewards(self) -> TT["n_transitions", torch.float] | None:
         if self._log_rewards is not None:
             return self._log_rewards
         if self.is_backward:
             return None
         else:
             log_rewards = torch.full(
                 (self.n_transitions,),
-                fill_value=-1.0,
+                fill_value=-float("inf"),
                 dtype=torch.float,
                 device=self.states.device,
             )
             try:
                 log_rewards[self.is_done] = self.env.log_reward(self.last_states)
             except NotImplementedError:
                 log_rewards[self.is_done] = torch.log(self.env.reward(self.last_states))
             return log_rewards
 
     @property
-    def all_log_rewards(self) -> PairFloatTensor:
-        """This is applicable to environments where all states are terminating.
-        This function evaluates the rewards for all transitions that do not end in the sink state.
-        This is useful for the Modified Detailed Balance loss."""
+    def all_log_rewards(self) -> TT["n_transitions", 2, torch.float]:
+        """Calculate all log rewards for the transitions.
+
+        This is applicable to environments where all states are terminating. This
+        function evaluates the rewards for all transitions that do not end in the sink
+        state. This is useful for the Modified Detailed Balance loss.
+
+        Raises:
+            NotImplementedError: when used for backward transitions.
+        """
         if self.is_backward:
             raise NotImplementedError("Not implemented for backward transitions")
         is_sink_state = self.next_states.is_sink_state
         log_rewards = torch.full(
             (self.n_transitions, 2),
-            fill_value=-1.0,
+            fill_value=-float("inf"),
             dtype=torch.float,
             device=self.states.device,
         )
         try:
             log_rewards[~is_sink_state, 0] = self.env.log_reward(
                 self.states[~is_sink_state]
             )
@@ -150,15 +174,15 @@
             )
             log_rewards[~is_sink_state, 1] = torch.log(
                 self.env.reward(self.next_states[~is_sink_state])
             )
         return log_rewards
 
     def __getitem__(self, index: int | Sequence[int]) -> Transitions:
-        "Access particular transitions of the batch."
+        """Access particular transitions of the batch."""
         if isinstance(index, int):
             index = [index]
         states = self.states[index]
         actions = self.actions[index]
         is_done = self.is_done[index]
         next_states = self.next_states[index]
         log_rewards = (
@@ -173,17 +197,17 @@
             next_states=next_states,
             is_backward=self.is_backward,
             log_rewards=log_rewards,
             log_probs=log_probs,
         )
 
     def extend(self, other: Transitions) -> None:
-        "Extend the Transitions object with another Transitions object."
+        """Extend the Transitions object with another Transitions object."""
         self.states.extend(other.states)
-        self.actions = torch.cat((self.actions, other.actions), dim=0)
+        self.actions.extend(other.actions)
         self.is_done = torch.cat((self.is_done, other.is_done), dim=0)
         self.next_states.extend(other.next_states)
         if self._log_rewards is not None and other._log_rewards is not None:
             self._log_rewards = torch.cat(
                 (self._log_rewards, other._log_rewards), dim=0
             )
         else:
```

### Comparing `torchgfn-0.2/src/gfn/envs/discrete_ebm.py` & `torchgfn-1.0.0/src/gfn/gym/discrete_ebm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 from abc import ABC, abstractmethod
 from typing import ClassVar, Literal, Tuple, cast
 
 import torch
 import torch.nn as nn
-from gymnasium.spaces import Discrete
-from torchtyping import TensorType
+from torchtyping import TensorType as TT
 
-from gfn.containers.states import States
-from gfn.envs.env import Env
-
-# Typing
-StatesTensor = TensorType["batch_shape", "state_shape", torch.float]
-BatchTensor = TensorType["batch_shape"]
-IsingJTensor = TensorType["state_shape", "state_shape", torch.float]
-ForwardMasksTensor = TensorType["batch_shape", "n_actions", torch.bool]
-BackwardMasksTensor = TensorType["batch_shape", "n_actions - 1", torch.bool]
+from gfn.actions import Actions
+from gfn.env import DiscreteEnv
+from gfn.preprocessors import EnumPreprocessor, IdentityPreprocessor
+from gfn.states import DiscreteStates, States
 
 
 class EnergyFunction(nn.Module, ABC):
     """Base class for energy functions"""
 
     @abstractmethod
-    def forward(self, states: StatesTensor) -> BatchTensor:
+    def forward(
+        self, states: TT["batch_shape", "state_shape", torch.float]
+    ) -> TT["batch_shape"]:
         pass
 
 
 class IsingModel(EnergyFunction):
     """Ising model energy function"""
 
-    def __init__(self, J: IsingJTensor):
+    def __init__(self, J: TT["state_shape", "state_shape", torch.float]):
         super().__init__()
         self.J = J
         self.linear = nn.Linear(J.shape[0], 1, bias=False)
         self.linear.weight.data = J
 
-    def forward(self, states: StatesTensor) -> BatchTensor:
+    def forward(
+        self, states: TT["batch_shape", "state_shape", torch.float]
+    ) -> TT["batch_shape"]:
         states = states.float()
         tmp = self.linear(states)
         return -(states * tmp).sum(-1)
 
 
-class DiscreteEBMEnv(Env):
+class DiscreteEBM(DiscreteEnv):
     """Environment for discrete energy-based models, based on https://arxiv.org/pdf/2202.01361.pdf"""
 
     def __init__(
         self,
         ndim: int,
         energy: EnergyFunction | None = None,
         alpha: float = 1.0,
         device_str: Literal["cpu", "cuda"] = "cpu",
+        preprocessor_name: Literal["Identity", "Enum"] = "Identity",
     ):
         """Discrete EBM environment.
 
         Args:
             ndim (int, optional): dimension D of the sampling space {0, 1}^D.
             energy (EnergyFunction): energy function of the EBM. Defaults to None. If None, the Ising model with Identity matrix is used.
             alpha (float, optional): interaction strength the EBM. Defaults to 1.0.
@@ -66,45 +65,64 @@
         if energy is None:
             energy = IsingModel(
                 torch.ones((ndim, ndim), device=torch.device(device_str))
             )
         self.energy: EnergyFunction = energy
         self.alpha = alpha
 
-        action_space = Discrete(
-            2 * ndim + 1
-        )  # the last action is the exit action that is only available for complete states
+        n_actions = 2 * ndim + 1
+        # the last action is the exit action that is only available for complete states
         # Action i in [0, ndim - 1] corresponds to replacing s[i] with 0
         # Action i in [ndim, 2 * ndim - 1] corresponds to replacing s[i - ndim] with 1
 
-        super().__init__(action_space=action_space, s0=s0, sf=sf)
+        if preprocessor_name == "Identity":
+            preprocessor = IdentityPreprocessor(output_dim=ndim)
+        elif preprocessor_name == "Enum":
+            preprocessor = EnumPreprocessor(
+                get_states_indices=self.get_states_indices,
+            )
+        else:
+            raise ValueError(f"Unknown preprocessor {preprocessor_name}")
 
-    def make_States_class(self) -> type[States]:
+        super().__init__(
+            n_actions=n_actions,
+            s0=s0,
+            sf=sf,
+            device_str=device_str,
+            preprocessor=preprocessor,
+        )
+
+    def make_States_class(self) -> type[DiscreteStates]:
         env = self
 
-        class DiscreteEBMStates(States):
+        class DiscreteEBMStates(DiscreteStates):
             state_shape: ClassVar[tuple[int, ...]] = (env.ndim,)
             s0 = env.s0
             sf = env.sf
+            n_actions = env.n_actions
+            device = env.device
 
             @classmethod
             def make_random_states_tensor(
                 cls, batch_shape: Tuple[int, ...]
-            ) -> StatesTensor:
+            ) -> TT["batch_shape", "state_shape", torch.float]:
                 return torch.randint(
                     -1,
                     2,
                     batch_shape + (env.ndim,),
                     dtype=torch.long,
                     device=env.device,
                 )
 
             def make_masks(
                 self,
-            ) -> Tuple[ForwardMasksTensor, BackwardMasksTensor]:
+            ) -> Tuple[
+                TT["batch_shape", "n_actions", torch.bool],
+                TT["batch_shape", "n_actions - 1", torch.bool],
+            ]:
                 forward_masks = torch.zeros(
                     self.batch_shape + (env.n_actions,),
                     device=env.device,
                     dtype=torch.bool,
                 )
                 backward_masks = torch.zeros(
                     self.batch_shape + (env.n_actions - 1,),
@@ -112,83 +130,105 @@
                     dtype=torch.bool,
                 )
 
                 return forward_masks, backward_masks
 
             def update_masks(self) -> None:
                 # The following two lines are for typing only.
-                self.forward_masks = cast(ForwardMasksTensor, self.forward_masks)
-                self.backward_masks = cast(BackwardMasksTensor, self.backward_masks)
-
-                self.forward_masks[..., : env.ndim] = self.states_tensor == -1
-                self.forward_masks[..., env.ndim : 2 * env.ndim] = (
-                    self.states_tensor == -1
-                )
-                self.forward_masks[..., -1] = torch.all(
-                    self.states_tensor != -1, dim=-1
-                )
-                self.backward_masks[..., : env.ndim] = self.states_tensor == 0
-                self.backward_masks[..., env.ndim : 2 * env.ndim] = (
-                    self.states_tensor == 1
+                self.forward_masks = cast(
+                    TT["batch_shape", "n_actions", torch.bool],
+                    self.forward_masks,
+                )
+                self.backward_masks = cast(
+                    TT["batch_shape", "n_actions - 1", torch.bool],
+                    self.backward_masks,
                 )
 
+                self.forward_masks[..., : env.ndim] = self.tensor == -1
+                self.forward_masks[..., env.ndim : 2 * env.ndim] = self.tensor == -1
+                self.forward_masks[..., -1] = torch.all(self.tensor != -1, dim=-1)
+                self.backward_masks[..., : env.ndim] = self.tensor == 0
+                self.backward_masks[..., env.ndim : 2 * env.ndim] = self.tensor == 1
+
         return DiscreteEBMStates
 
-    def is_exit_actions(self, actions: BatchTensor) -> BatchTensor:
+    def is_exit_actions(self, actions: TT["batch_shape"]) -> TT["batch_shape"]:
         return actions == self.n_actions - 1
 
-    def maskless_step(self, states: StatesTensor, actions: BatchTensor) -> None:
-        # First, we select that actions that replace a -1 with a 0
-        mask_0 = actions < self.ndim
-        states[mask_0] = states[mask_0].scatter(-1, actions[mask_0].unsqueeze(-1), 0)
-        # Then, we select that actions that replace a -1 with a 1
-        mask_1 = (actions >= self.ndim) & (actions < 2 * self.ndim)
-        states[mask_1] = states[mask_1].scatter(
-            -1, (actions[mask_1] - self.ndim).unsqueeze(-1), 1
+    def maskless_step(
+        self, states: States, actions: Actions
+    ) -> TT["batch_shape", "state_shape", torch.float]:
+        # First, we select that actions that replace a -1 with a 0.
+        # Remove singleton dimension for broadcasting.
+        mask_0 = (actions.tensor < self.ndim).squeeze(-1)
+        states.tensor[mask_0] = states.tensor[mask_0].scatter(
+            -1, actions.tensor[mask_0], 0  # Set indices to 0.
         )
+        # Then, we select that actions that replace a -1 with a 1.
+        mask_1 = (
+            (actions.tensor >= self.ndim) & (actions.tensor < 2 * self.ndim)
+        ).squeeze(
+            -1
+        )  # Remove singleton dimension for broadcasting.
+        states.tensor[mask_1] = states.tensor[mask_1].scatter(
+            -1, (actions.tensor[mask_1] - self.ndim), 1  # Set indices to 1.
+        )
+        return states.tensor
 
     def maskless_backward_step(
-        self, states: StatesTensor, actions: BatchTensor
-    ) -> None:
-        states.scatter_(-1, actions.unsqueeze(-1).fmod(self.ndim), -1)
+        self, states: States, actions: Actions
+    ) -> TT["batch_shape", "state_shape", torch.float]:
+        # In this env, states are n-dim vectors. s0 is empty (represented as -1),
+        # so s0=[-1, -1, ..., -1], each action is replacing a -1 with either a
+        # 0 or 1. Action i in [0, ndim-1] os replacing s[i] with 0, whereas
+        # action i in [ndim, 2*ndim-1] corresponds to replacing s[i - ndim] with 1.
+        # A backward action asks "what index should be set back to -1", hence the fmod
+        # to enable wrapping of indices.
+        return states.tensor.scatter(
+            -1,
+            actions.tensor.fmod(self.ndim),
+            -1,
+        )
 
-    def log_reward(self, final_states: States) -> BatchTensor:
-        raw_states = final_states.states_tensor
+    def log_reward(self, final_states: DiscreteStates) -> TT["batch_shape"]:
+        raw_states = final_states.tensor
         canonical = 2 * raw_states - 1
         return -self.alpha * self.energy(canonical)
 
-    def get_states_indices(self, states: States) -> BatchTensor:
+    def get_states_indices(self, states: DiscreteStates) -> TT["batch_shape"]:
         """The chosen encoding is the following: -1 -> 0, 0 -> 1, 1 -> 2, then we convert to base 3"""
-        states_raw = states.states_tensor
+        states_raw = states.tensor
         canonical_base = 3 ** torch.arange(self.ndim - 1, -1, -1, device=self.device)
         return (states_raw + 1).mul(canonical_base).sum(-1).long()
 
-    def get_terminating_states_indices(self, states: States) -> BatchTensor:
-        states_raw = states.states_tensor
+    def get_terminating_states_indices(
+        self, states: DiscreteStates
+    ) -> TT["batch_shape"]:
+        states_raw = states.tensor
         canonical_base = 2 ** torch.arange(self.ndim - 1, -1, -1, device=self.device)
         return (states_raw).mul(canonical_base).sum(-1).long()
 
     @property
     def n_states(self) -> int:
         return 3**self.ndim
 
     @property
     def n_terminating_states(self) -> int:
         return 2**self.ndim
 
     @property
-    def all_states(self) -> States:
+    def all_states(self) -> DiscreteStates:
         # This is brute force !
         digits = torch.arange(3, device=self.device)
         all_states = torch.cartesian_prod(*[digits] * self.ndim)
         all_states = all_states - 1
         return self.States(all_states)
 
     @property
-    def terminating_states(self) -> States:
+    def terminating_states(self) -> DiscreteStates:
         digits = torch.arange(2, device=self.device)
         all_states = torch.cartesian_prod(*[digits] * self.ndim)
         return self.States(all_states)
 
     @property
     def true_dist_pmf(self) -> torch.Tensor:
         true_dist = self.reward(self.terminating_states)
```

### Comparing `torchgfn-0.2/src/gfn/envs/env.py` & `torchgfn-1.0.0/src/gfn/env.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,215 +1,313 @@
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from typing import Optional, Tuple, Union
 
 import torch
-from gymnasium.spaces import Discrete, Space
-from torchtyping import TensorType
+from torchtyping import TensorType as TT
 
-from gfn.containers.states import States, correct_cast
-from gfn.envs.preprocessors import IdentityPreprocessor, Preprocessor
-
-# Typing
-TensorLong = TensorType["batch_shape", torch.long]
-TensorFloat = TensorType["batch_shape", torch.float]
-TensorBool = TensorType["batch_shape", torch.bool]
-ForwardMasksTensor = TensorType["batch_shape", "n_actions", torch.bool]
-BackwardMasksTensor = TensorType["batch_shape", "n_actions - 1", torch.bool]
-OneStateTensor = TensorType["state_shape", torch.float]
-StatesTensor = TensorType["batch_shape", "state_shape", torch.float]
-PmfTensor = TensorType["n_states", torch.float]
+from gfn.actions import Actions
+from gfn.preprocessors import IdentityPreprocessor, Preprocessor
+from gfn.states import DiscreteStates, States
 
+# Errors
 NonValidActionsError = type("NonValidActionsError", (ValueError,), {})
 
 
 class Env(ABC):
-    """
-    Base class for environments, showing which methods should be implemented.
-    A common assumption for all environments is that all actions are discrete,
-    represented by a number in {0, ..., n_actions - 1}, the last one being the
-    exit action.
-    """
+    """Base class for all environments. Environments require that individual states be represented as a unique tensor of
+    arbitrary shape."""
 
     def __init__(
         self,
-        action_space: Space,
-        s0: OneStateTensor,
-        sf: Optional[OneStateTensor] = None,
+        s0: TT["state_shape", torch.float],
+        sf: Optional[TT["state_shape", torch.float]] = None,
         device_str: Optional[str] = None,
         preprocessor: Optional[Preprocessor] = None,
     ):
-        self.s0 = s0
+        """Initializes an environment.
+
+        Args:
+            s0: Representation of the initial state. All individual states would be of the same shape.
+            sf (optional): Representation of the final state. Only used for a human readable representation of
+                the states or trajectories.
+            device_str (Optional[str], optional): 'cpu' or 'cuda'. Defaults to None, in which case the device is inferred from s0.
+            preprocessor (Optional[Preprocessor], optional): a Preprocessor object that converts raw states to a tensor that can be fed
+                into a neural network. Defaults to None, in which case the IdentityPreprocessor is used.
+        """
+        self.device = torch.device(device_str) if device_str is not None else s0.device
+
+        self.s0 = s0.to(self.device)
         if sf is None:
-            sf = torch.full(s0.shape, -float("inf"))
+            sf = torch.full(s0.shape, -float("inf")).to(self.device)
         self.sf = sf
-        self.action_space = action_space
-        self.device = torch.device(device_str) if device_str is not None else s0.device
+
         self.States = self.make_States_class()
+        self.Actions = self.make_Actions_class()
 
         if preprocessor is None:
-            preprocessor = IdentityPreprocessor(output_shape=tuple(s0.shape))
+            assert (
+                s0.ndim == 1
+            ), "The default preprocessor can only be used for uni-dimensional states."
+            output_dim = s0.shape[0]
+            preprocessor = IdentityPreprocessor(output_dim=output_dim)
 
         self.preprocessor = preprocessor
+        self.is_discrete = False
 
     @abstractmethod
     def make_States_class(self) -> type[States]:
-        "Returns a class that inherits from States and implements the environment-specific methods."
+        """Returns a class that inherits from States and implements the environment-specific methods."""
+        pass
+
+    @abstractmethod
+    def make_Actions_class(self) -> type[Actions]:
+        """Returns a class that inherits from Actions and implements the environment-specific methods."""
         pass
 
+    def reset(
+        self,
+        batch_shape: Optional[Union[int, Tuple[int]]] = None,
+        random: bool = False,
+        sink: bool = False,
+        seed: int = None,
+    ) -> States:
+        """
+        Instantiates a batch of initial states. random and sink cannot be both True.
+        When random is true and seed is not None, environment randomization is fixed by
+        the submitted seed for reproducibility.
+        """
+        assert not (random and sink)
+
+        if random and seed is not None:
+            torch.manual_seed(seed)
+
+        if batch_shape is None:
+            batch_shape = (1,)
+        if isinstance(batch_shape, int):
+            batch_shape = (batch_shape,)
+        return self.States.from_batch_shape(
+            batch_shape=batch_shape, random=random, sink=sink
+        )
+
     @abstractmethod
-    def is_exit_actions(self, actions: TensorLong) -> TensorBool:
-        "Returns True if the action is an exit action."
+    def maskless_step(
+        self, states: States, actions: Actions
+    ) -> TT["batch_shape", "state_shape", torch.float]:
+        """Function that takes a batch of states and actions and returns a batch of next
+        states. Does not need to check whether the actions are valid or the states are sink states.
+        """
         pass
 
     @abstractmethod
-    def maskless_step(self, states: StatesTensor, actions: TensorLong) -> None:
-        """Same as the step function, but without worrying whether or not the actions are valid, or masking."""
+    def maskless_backward_step(
+        self, states: States, actions: Actions
+    ) -> TT["batch_shape", "state_shape", torch.float]:
+        """Function that takes a batch of states and actions and returns a batch of previous
+        states. Does not need to check whether the actions are valid or the states are sink states.
+        """
         pass
 
     @abstractmethod
-    def maskless_backward_step(self, states: StatesTensor, actions: TensorLong) -> None:
-        """Same as the backward_step function, but without worrying whether or not the actions are valid, or masking."""
+    def is_action_valid(
+        self,
+        states: States,
+        actions: Actions,
+        backward: bool = False,
+    ) -> bool:
+        """Returns True if the actions are valid in the given states."""
         pass
 
-    def reward(self, final_states: States) -> TensorFloat:
+    def validate_actions(
+        self, states: States, actions: Actions, backward: bool = False
+    ) -> bool:
+        """First, asserts that states and actions have the same batch_shape.
+        Then, uses `is_action_valid`.
+        Returns a boolean indicating whether states/actions pairs are valid."""
+        assert states.batch_shape == actions.batch_shape
+        return self.is_action_valid(states, actions, backward)
+
+    def step(
+        self,
+        states: States,
+        actions: Actions,
+    ) -> States:
+        """Function that takes a batch of states and actions and returns a batch of next
+        states and a boolean tensor indicating sink states in the new batch."""
+        new_states = deepcopy(states)
+        valid_states_idx: TT["batch_shape", torch.bool] = ~states.is_sink_state
+        valid_actions = actions[valid_states_idx]
+        valid_states = states[valid_states_idx]
+
+        if not self.validate_actions(valid_states, valid_actions):
+            raise NonValidActionsError(
+                "Some actions are not valid in the given states. See `is_action_valid`."
+            )
+
+        new_sink_states_idx = actions.is_exit
+        new_states.tensor[new_sink_states_idx] = self.sf
+        new_sink_states_idx = ~valid_states_idx | new_sink_states_idx
+
+        not_done_states = new_states[~new_sink_states_idx]
+        not_done_actions = actions[~new_sink_states_idx]
+
+        new_not_done_states_tensor = self.maskless_step(
+            not_done_states, not_done_actions
+        )
+        # if isinstance(new_states, DiscreteStates):
+        #     new_not_done_states.masks = self.update_masks(not_done_states, not_done_actions)
+
+        new_states.tensor[~new_sink_states_idx] = new_not_done_states_tensor
+
+        return new_states
+
+    def backward_step(
+        self,
+        states: States,
+        actions: Actions,
+    ) -> States:
+        """Function that takes a batch of states and actions and returns a batch of next
+        states and a boolean tensor indicating initial states in the new batch."""
+        new_states = deepcopy(states)
+        valid_states_idx: TT["batch_shape", torch.bool] = ~new_states.is_initial_state
+        valid_actions = actions[valid_states_idx]
+        valid_states = states[valid_states_idx]
+
+        if not self.validate_actions(valid_states, valid_actions, backward=True):
+            raise NonValidActionsError(
+                "Some actions are not valid in the given states. See `is_action_valid`."
+            )
+
+        # Calculate the backward step, and update only the states which are not Done.
+        new_not_done_states_tensor = self.maskless_backward_step(
+            valid_states, valid_actions
+        )
+        new_states.tensor[valid_states_idx] = new_not_done_states_tensor
+
+        if isinstance(new_states, DiscreteStates):
+            new_states.update_masks()
+
+        return new_states
+
+    def reward(self, final_states: States) -> TT["batch_shape", torch.float]:
         """Either this or log_reward needs to be implemented."""
         return torch.exp(self.log_reward(final_states))
 
-    def log_reward(self, final_states: States) -> TensorFloat:
+    def log_reward(self, final_states: States) -> TT["batch_shape", torch.float]:
         """Either this or reward needs to be implemented."""
         raise NotImplementedError("log_reward function not implemented")
 
-    def get_states_indices(self, states: States) -> TensorLong:
+    @property
+    def log_partition(self) -> float:
+        "Returns the logarithm of the partition function."
         return NotImplementedError(
             "The environment does not support enumeration of states"
         )
 
-    def get_terminating_states_indices(self, states: States) -> TensorLong:
+
+class DiscreteEnv(Env, ABC):
+    """
+    Base class for discrete environments, where actions are represented by a number in
+    {0, ..., n_actions - 1}, the last one being the exit action.
+    `DiscreteEnv` allow specifying the validity of actions (forward and backward), via mask tensors, that
+    are directly attached to `States` objects.
+    """
+
+    def __init__(
+        self,
+        n_actions: int,
+        s0: TT["state_shape", torch.float],
+        sf: Optional[TT["state_shape", torch.float]] = None,
+        device_str: Optional[str] = None,
+        preprocessor: Optional[Preprocessor] = None,
+    ):
+        """Initializes a discrete environment.
+
+        Args:
+            n_actions: The number of actions in the environment.
+
+        """
+        self.n_actions = n_actions
+        super().__init__(s0, sf, device_str, preprocessor)
+        self.is_discrete = True
+
+    def make_Actions_class(self) -> type[Actions]:
+        env = self
+        n_actions = self.n_actions
+
+        class DiscreteEnvActions(Actions):
+            action_shape = (1,)
+            dummy_action = torch.tensor([-1], device=env.device)  # Double check
+            exit_action = torch.tensor([n_actions - 1], device=env.device)
+
+        return DiscreteEnvActions
+
+    def is_action_valid(
+        self, states: States, actions: Actions, backward: bool = False
+    ) -> bool:
+        assert states.forward_masks is not None and states.backward_masks is not None
+        masks_tensor = states.backward_masks if backward else states.forward_masks
+        return torch.gather(masks_tensor, 1, actions.tensor).all()
+
+    def step(
+        self,
+        states: DiscreteStates,
+        actions: Actions,
+    ) -> States:
+        new_states = super().step(states, actions)
+        new_states.update_masks()
+        return new_states
+
+    def get_states_indices(
+        self, states: DiscreteStates
+    ) -> TT["batch_shape", torch.long]:
         return NotImplementedError(
             "The environment does not support enumeration of states"
         )
 
-    @property
-    def n_actions(self) -> int:
-        if isinstance(self.action_space, Discrete):
-            return self.action_space.n
-        else:
-            raise NotImplementedError("Only discrete action spaces are supported")
-
-    @property
-    def n_states(self) -> int:
+    def get_terminating_states_indices(
+        self, states: DiscreteStates
+    ) -> TT["batch_shape", torch.long]:
         return NotImplementedError(
             "The environment does not support enumeration of states"
         )
 
     @property
-    def n_terminating_states(self) -> int:
+    def n_states(self) -> int:
         return NotImplementedError(
             "The environment does not support enumeration of states"
         )
 
     @property
-    def true_dist_pmf(self) -> PmfTensor:
-        "Returns a one-dimensional tensor representing the true distribution."
+    def n_terminating_states(self) -> int:
         return NotImplementedError(
             "The environment does not support enumeration of states"
         )
 
     @property
-    def log_partition(self) -> float:
-        "Returns the logarithm of the partition function."
+    def true_dist_pmf(self) -> TT["n_states", torch.float]:
+        "Returns a one-dimensional tensor representing the true distribution."
         return NotImplementedError(
             "The environment does not support enumeration of states"
         )
 
     @property
-    def all_states(self) -> States:
-        """Returns a batch of all states for environments with enumerable states.
+    def all_states(self) -> DiscreteStates:
+        """Returns a batch of all states.
         The batch_shape should be (n_states,).
         This should satisfy:
         self.get_states_indices(self.all_states) == torch.arange(self.n_states)
         """
         return NotImplementedError(
             "The environment does not support enumeration of states"
         )
 
     @property
-    def terminating_states(self) -> States:
+    def terminating_states(self) -> DiscreteStates:
         """Returns a batch of all terminating states for environments with enumerable states.
         The batch_shape should be (n_terminating_states,).
         This should satisfy:
         self.get_terminating_states_indices(self.terminating_states) == torch.arange(self.n_terminating_states)
         """
         return NotImplementedError(
             "The environment does not support enumeration of states"
         )
-
-    def reset(
-        self, batch_shape: Union[int, Tuple[int]], random: bool = False
-    ) -> States:
-        "Instantiates a batch of initial states."
-        if isinstance(batch_shape, int):
-            batch_shape = (batch_shape,)
-        return self.States.from_batch_shape(batch_shape=batch_shape, random=random)
-
-    def step(
-        self,
-        states: States,
-        actions: TensorLong,
-    ) -> States:
-        """Function that takes a batch of states and actions and returns a batch of next
-        states and a boolean tensor indicating sink states in the new batch."""
-        new_states = deepcopy(states)
-        valid_states: TensorBool = ~states.is_sink_state
-        valid_actions = actions[valid_states]
-
-        if new_states.forward_masks is not None:
-            new_forward_masks, _ = correct_cast(
-                new_states.forward_masks, new_states.backward_masks
-            )
-            valid_states_masks = new_forward_masks[valid_states]
-            valid_actions_bool = all(
-                torch.gather(valid_states_masks, 1, valid_actions.unsqueeze(1))
-            )
-            if not valid_actions_bool:
-                raise NonValidActionsError("Actions are not valid")
-
-        new_sink_states = self.is_exit_actions(actions)
-        new_states.states_tensor[new_sink_states] = self.sf
-        new_sink_states = ~valid_states | new_sink_states
-
-        not_done_states = new_states.states_tensor[~new_sink_states]
-        not_done_actions = actions[~new_sink_states]
-
-        self.maskless_step(not_done_states, not_done_actions)
-
-        new_states.states_tensor[~new_sink_states] = not_done_states
-
-        new_states.update_masks()
-        return new_states
-
-    def backward_step(self, states: States, actions: TensorLong) -> States:
-        """Function that takes a batch of states and actions and returns a batch of next
-        states and a boolean tensor indicating initial states in the new batch."""
-        new_states = deepcopy(states)
-        valid_states: TensorBool = ~new_states.is_initial_state
-        valid_actions = actions[valid_states]
-
-        if new_states.backward_masks is not None:
-            _, new_backward_masks = correct_cast(
-                new_states.forward_masks, new_states.backward_masks
-            )
-            valid_states_masks = new_backward_masks[valid_states]
-            valid_actions_bool = all(
-                torch.gather(valid_states_masks, 1, valid_actions.unsqueeze(1))
-            )
-            if not valid_actions_bool:
-                raise NonValidActionsError("Actions are not valid")
-
-        not_done_states = new_states.states_tensor[valid_states]
-        self.maskless_backward_step(not_done_states, valid_actions)
-
-        new_states.states_tensor[valid_states] = not_done_states
-
-        new_states.update_masks()
-        return new_states
```

### Comparing `torchgfn-0.2/src/gfn/envs/hypergrid.py` & `torchgfn-1.0.0/src/gfn/gym/hypergrid.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,34 @@
 """
 Copied and Adapted from https://github.com/Tikquuss/GflowNets_Tutorial
 """
-
 from typing import ClassVar, Literal, Tuple, cast
 
 import torch
 from einops import rearrange
-from gymnasium.spaces import Discrete
-from torchtyping import TensorType
+from torchtyping import TensorType as TT
 
-from gfn.containers.states import States
-from gfn.envs.env import Env
-from gfn.envs.preprocessors import (
-    IdentityPreprocessor,
-    KHotPreprocessor,
-    OneHotPreprocessor,
-)
-
-# Typing
-TensorLong = TensorType["batch_shape", torch.long]
-TensorFloat = TensorType["batch_shape", torch.float]
-TensorBool = TensorType["batch_shape", torch.bool]
-ForwardMasksTensor = TensorType["batch_shape", "n_actions", torch.bool]
-BackwardMasksTensor = TensorType["batch_shape", "n_actions - 1", torch.bool]
-OneStateTensor = TensorType["state_shape", torch.float]
-StatesTensor = TensorType["batch_shape", "state_shape", torch.float]
-
-preprocessors_dict = {
-    "KHot": KHotPreprocessor,
-    "OneHot": OneHotPreprocessor,
-    "Identity": IdentityPreprocessor,
-}
+from gfn.actions import Actions
+from gfn.env import DiscreteEnv
+from gfn.gym.helpers.preprocessors import KHotPreprocessor, OneHotPreprocessor
+from gfn.preprocessors import EnumPreprocessor, IdentityPreprocessor
+from gfn.states import DiscreteStates
 
 
-class HyperGrid(Env):
+class HyperGrid(DiscreteEnv):
     def __init__(
         self,
         ndim: int = 2,
         height: int = 4,
         R0: float = 0.1,
         R1: float = 0.5,
         R2: float = 2.0,
         reward_cos: bool = False,
         device_str: Literal["cpu", "cuda"] = "cpu",
-        preprocessor_name: Literal["KHot", "OneHot", "Identity"] = "KHot",
+        preprocessor_name: Literal["KHot", "OneHot", "Identity", "Enum"] = "KHot",
     ):
         """HyperGrid environment from the GFlowNets paper.
         The states are represented as 1-d tensors of length `ndim` with values in
         {0, 1, ..., height - 1}.
         A preprocessor transforms the states to the input of the neural network,
         which can be a one-hot, a K-hot, or an identity encoding.
 
@@ -69,120 +50,132 @@
         self.reward_cos = reward_cos
 
         s0 = torch.zeros(ndim, dtype=torch.long, device=torch.device(device_str))
         sf = torch.full(
             (ndim,), fill_value=-1, dtype=torch.long, device=torch.device(device_str)
         )
 
-        action_space = Discrete(ndim + 1)
+        n_actions = ndim + 1
 
         if preprocessor_name == "Identity":
-            preprocessor = IdentityPreprocessor(output_shape=(ndim,))
+            preprocessor = IdentityPreprocessor(output_dim=ndim)
         elif preprocessor_name == "KHot":
             preprocessor = KHotPreprocessor(
                 height=height, ndim=ndim, get_states_indices=self.get_states_indices
             )
         elif preprocessor_name == "OneHot":
             preprocessor = OneHotPreprocessor(
                 n_states=self.n_states,
                 get_states_indices=self.get_states_indices,
             )
+        elif preprocessor_name == "Enum":
+            preprocessor = EnumPreprocessor(
+                get_states_indices=self.get_states_indices,
+            )
         else:
             raise ValueError(f"Unknown preprocessor {preprocessor_name}")
 
         super().__init__(
-            action_space=action_space,
+            n_actions=n_actions,
             s0=s0,
             sf=sf,
             device_str=device_str,
             preprocessor=preprocessor,
         )
 
-    def make_States_class(self) -> type[States]:
+    def make_States_class(self) -> type[DiscreteStates]:
         "Creates a States class for this environment"
         env = self
 
-        class HyperGridStates(States):
-
+        class HyperGridStates(DiscreteStates):
             state_shape: ClassVar[tuple[int, ...]] = (env.ndim,)
             s0 = env.s0
             sf = env.sf
+            n_actions = env.n_actions
+            device = env.device
 
             @classmethod
             def make_random_states_tensor(
                 cls, batch_shape: Tuple[int, ...]
-            ) -> StatesTensor:
+            ) -> TT["batch_shape", "state_shape", torch.float]:
                 "Creates a batch of random states."
                 states_tensor = torch.randint(
                     0, env.height, batch_shape + env.s0.shape, device=env.device
                 )
                 return states_tensor
 
-            def make_masks(self) -> Tuple[ForwardMasksTensor, BackwardMasksTensor]:
-                "Mask illegal (forward and backward) actions."
-                forward_masks = torch.ones(
-                    (*self.batch_shape, env.n_actions),
-                    dtype=torch.bool,
-                    device=env.device,
-                )
-                backward_masks = torch.ones(
-                    (*self.batch_shape, env.n_actions - 1),
-                    dtype=torch.bool,
-                    device=env.device,
-                )
-
-                return forward_masks, backward_masks
-
             def update_masks(self) -> None:
                 "Update the masks based on the current states."
                 # The following two lines are for typing only.
-                self.forward_masks = cast(ForwardMasksTensor, self.forward_masks)
-                self.backward_masks = cast(BackwardMasksTensor, self.backward_masks)
+                self.forward_masks = cast(
+                    TT["batch_shape", "n_actions", torch.bool],
+                    self.forward_masks,
+                )
+                self.backward_masks = cast(
+                    TT["batch_shape", "n_actions - 1", torch.bool],
+                    self.backward_masks,
+                )
 
-                self.forward_masks[..., :-1] = self.states_tensor != env.height - 1
-                self.backward_masks = self.states_tensor != 0
+                self.forward_masks[..., :-1] = self.tensor != env.height - 1
+                self.backward_masks = self.tensor != 0
 
         return HyperGridStates
 
-    def is_exit_actions(self, actions: TensorLong) -> TensorBool:
-        return actions == self.action_space.n - 1
-
-    def maskless_step(self, states: StatesTensor, actions: TensorLong) -> None:
-        states.scatter_(-1, actions.unsqueeze(-1), 1, reduce="add")
-
-    def maskless_backward_step(self, states: StatesTensor, actions: TensorLong) -> None:
-        states.scatter_(-1, actions.unsqueeze(-1), -1, reduce="add")
-
-    def true_reward(self, final_states: States) -> TensorFloat:
-        final_states_raw = final_states.states_tensor
+    def maskless_step(
+        self, states: DiscreteStates, actions: Actions
+    ) -> TT["batch_shape", "state_shape", torch.float]:
+        new_states_tensor = states.tensor.scatter(-1, actions.tensor, 1, reduce="add")
+        return new_states_tensor
+
+    def maskless_backward_step(
+        self, states: DiscreteStates, actions: Actions
+    ) -> TT["batch_shape", "state_shape", torch.float]:
+        new_states_tensor = states.tensor.scatter(-1, actions.tensor, -1, reduce="add")
+        return new_states_tensor
+
+    def true_reward(
+        self, final_states: DiscreteStates
+    ) -> TT["batch_shape", torch.float]:
+        r"""In the normal setting, the reward is:
+        R(s) = R_0 + 0.5 \prod_{d=1}^D \mathbf{1} \left( \left\lvert \frac{s^d}{H-1}
+          - 0.5 \right\rvert \in (0.25, 0.5] \right)
+          + 2 \prod_{d=1}^D \mathbf{1} \left( \left\lvert \frac{s^d}{H-1} - 0.5 \right\rvert \in (0.3, 0.4) \right)
+        """
+        final_states_raw = final_states.tensor
         R0, R1, R2 = (self.R0, self.R1, self.R2)
         ax = abs(final_states_raw / (self.height - 1) - 0.5)
         if not self.reward_cos:
             reward = (
                 R0 + (0.25 < ax).prod(-1) * R1 + ((0.3 < ax) * (ax < 0.4)).prod(-1) * R2
             )
         else:
             pdf_input = ax * 5
             pdf = 1.0 / (2 * torch.pi) ** 0.5 * torch.exp(-(pdf_input**2) / 2)
             reward = R0 + ((torch.cos(ax * 50) + 1) * pdf).prod(-1) * R1
         return reward
 
-    def log_reward(self, final_states: States) -> TensorFloat:
+    def log_reward(
+        self, final_states: DiscreteStates
+    ) -> TT["batch_shape", torch.float]:
         return torch.log(self.true_reward(final_states))
 
-    def get_states_indices(self, states: States) -> TensorLong:
-        states_raw = states.states_tensor
+    def get_states_indices(
+        self, states: DiscreteStates
+    ) -> TT["batch_shape", torch.long]:
+        states_raw = states.tensor
 
         canonical_base = self.height ** torch.arange(
             self.ndim - 1, -1, -1, device=states_raw.device
         )
         indices = (canonical_base * states_raw).sum(-1).long()
         return indices
 
-    def get_terminating_states_indices(self, states: States) -> TensorLong:
+    def get_terminating_states_indices(
+        self, states: DiscreteStates
+    ) -> TT["batch_shape", torch.long]:
         return self.get_states_indices(states)
 
     @property
     def n_states(self) -> int:
         return self.height**self.ndim
 
     @property
@@ -202,15 +195,15 @@
 
     @property
     def log_partition(self) -> float:
         grid = self.build_grid()
         rewards = self.reward(grid)
         return rewards.sum().log().item()
 
-    def build_grid(self) -> States:
+    def build_grid(self) -> DiscreteStates:
         "Utility function to build the complete grid"
         H = self.height
         ndim = self.ndim
         grid_shape = (H,) * ndim + (ndim,)  # (H, ..., H, ndim)
         grid = torch.zeros(grid_shape, device=self.device)
         for i in range(ndim):
             grid_i = torch.linspace(start=0, end=H - 1, steps=H)
@@ -222,15 +215,15 @@
         rearrange_string += " ndim -> "
         rearrange_string += " ".join([f"n{i}" for i in range(ndim, 0, -1)])
         rearrange_string += " ndim"
         grid = rearrange(grid, rearrange_string).long()
         return self.States(grid)
 
     @property
-    def all_states(self) -> States:
+    def all_states(self) -> DiscreteStates:
         grid = self.build_grid()
-        flat_grid = rearrange(grid.states_tensor, "... ndim -> (...) ndim")
+        flat_grid = rearrange(grid.tensor, "... ndim -> (...) ndim")
         return self.States(flat_grid)
 
     @property
-    def terminating_states(self) -> States:
+    def terminating_states(self) -> DiscreteStates:
         return self.all_states
```

### Comparing `torchgfn-0.2/src/gfn/envs/preprocessors/base.py` & `torchgfn-1.0.0/src/gfn/preprocessors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,54 @@
 from abc import ABC, abstractmethod
 from typing import Callable, Tuple
 
-from torchtyping import TensorType
+from torchtyping import TensorType as TT
 
-from gfn.containers import States
-
-# Typing
-OutputTensor = TensorType["batch_shape", "dim_in"]
+from gfn.states import States
 
 
 class Preprocessor(ABC):
     """
     Base class for Preprocessors. The goal is to transform tensors representing raw states
     to tensors that can be used as input to neural networks.
     """
 
-    name: str = "Preprocessor"
-
-    def __init__(self, output_shape: Tuple[int]) -> None:
-        self.output_shape = output_shape
+    def __init__(self, output_dim: int) -> None:
+        self.output_dim = output_dim
 
     @abstractmethod
-    def preprocess(self, states: States) -> OutputTensor:
+    def preprocess(self, states: States) -> TT["batch_shape", "input_dim"]:
         pass
 
-    def __call__(self, states: States) -> OutputTensor:
+    def __call__(self, states: States) -> TT["batch_shape", "input_dim"]:
         return self.preprocess(states)
 
     def __repr__(self):
-        return f"{self.name}, output_shape={self.output_shape}"
+        return f"{self.__class__.__name__}, output_dim={self.output_dim}"
 
 
 class IdentityPreprocessor(Preprocessor):
     """Simple preprocessor applicable to environments with uni-dimensional states.
     This is the default preprocessor used."""
 
-    name = "IdentityPreprocessor"
-
-    def preprocess(self, states: States) -> OutputTensor:
-        return states.states_tensor.float()
+    def preprocess(self, states: States) -> TT["batch_shape", "input_dim"]:
+        return states.tensor.float()
 
 
 class EnumPreprocessor(Preprocessor):
     "Preprocessor applicable to environments with discrete states."
-    name = "EnumPreprocessor"
 
-    def __init__(self, get_states_indices: Callable[[States], OutputTensor]) -> None:
+    def __init__(
+        self,
+        get_states_indices: Callable[[States], TT["batch_shape", "input_dim"]],
+    ) -> None:
         """Preprocessor for environments with enumerable states (finite number of states).
         Each state is represented by a unique integer (>= 0) index.
 
         Args:
-            get_states_indices (Callable[[States], OutputTensor]): function that returns the unique indices of the states.
+            get_states_indices (Callable[[States], BatchOutputTensor]): function that returns the unique indices of the states.
         """
-        super().__init__(output_shape=(1,))
+        super().__init__(output_dim=1)
         self.get_states_indices = get_states_indices
 
     def preprocess(self, states):
         return self.get_states_indices(states).long().unsqueeze(-1)
```

### Comparing `torchgfn-0.2/src/gfn/envs/preprocessors/hot.py` & `torchgfn-1.0.0/src/gfn/gym/helpers/preprocessors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,60 @@
 from typing import Callable
 
 import torch
 from einops import rearrange
 from torch.nn.functional import one_hot
-from torchtyping import TensorType
+from torchtyping import TensorType as TT
 
-from gfn.containers.states import States
-from gfn.envs.preprocessors.base import Preprocessor
-
-# Typing
-OutputTensor = TensorType["batch_shape", "dim_in"]
+from gfn.preprocessors import Preprocessor
+from gfn.states import States
 
 
 class OneHotPreprocessor(Preprocessor):
-    name = "one_hot"
-
     def __init__(
         self,
         n_states: int,
-        get_states_indices: Callable[[States], OutputTensor],
+        get_states_indices: Callable[[States], TT["batch_shape", "input_dim"]],
     ) -> None:
         """One Hot Preprocessor for environments with enumerable states (finite number of states).
 
         Args:
             n_states (int): The total number of states in the environment (not including s_f).
-            get_states_indices (Callable[[States], OutputTensor]): function that returns the unique indices of the states.
+            get_states_indices (Callable[[States], BatchOutputTensor]): function that returns the unique indices of the states.
         """
-        super().__init__(output_shape=(n_states,))
+        super().__init__(output_dim=n_states)
         self.get_states_indices = get_states_indices
         self.output_dim = n_states
 
     def preprocess(self, states):
         state_indices = self.get_states_indices(states)
         return one_hot(state_indices, self.output_dim).float()
 
 
 class KHotPreprocessor(Preprocessor):
-    name = "k_hot"
-
     def __init__(
         self,
         height: int,
         ndim: int,
-        get_states_indices: Callable[[States], OutputTensor],
+        get_states_indices: Callable[[States], TT["batch_shape", "input_dim"]],
     ) -> None:
         """K Hot Preprocessor for environments with enumerable states (finite number of states) with a grid structure.
 
         Args:
             height (int): number of unique values per dimension.
             ndim (int): number of dimensions.
-            get_states_indices (Callable[[States], OutputTensor]): function that returns the unique indices of the states.
+            get_states_indices (Callable[[States], BatchOutputTensor]): function that returns the unique indices of the states.
         """
-        super().__init__(output_shape=(height * ndim,))
+        super().__init__(output_dim=height * ndim)
         self.height = height
         self.ndim = ndim
         self.get_states_indices = get_states_indices
 
     def preprocess(self, states):
-        states_tensor = states.states_tensor
+        states_tensor = states.tensor
         assert (
             states_tensor.dtype == torch.long
         ), "K Hot preprocessing only works for integer states"
         states_tensor = states_tensor.long()
         hot = one_hot(states_tensor, self.height).float()
         hot = rearrange(hot, "... a b -> ... (a b)")
         return hot
```

### Comparing `torchgfn-0.2/src/gfn/losses/detailed_balance.py` & `torchgfn-1.0.0/src/gfn/gflownet/detailed_balance.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,104 @@
-from dataclasses import dataclass
+from typing import Tuple
 
 import torch
-from torchtyping import TensorType
+from torchtyping import TensorType as TT
 
-from gfn.containers import Transitions
-from gfn.estimators import LogStateFlowEstimator
-from gfn.losses.base import EdgeDecomposableLoss, PFBasedParametrization
-from gfn.samplers.actions_samplers import (
-    BackwardDiscreteActionsSampler,
-    DiscreteActionsSampler,
-)
-
-# Typing
-ScoresTensor = TensorType["n_transitions", float]
-LossTensor = TensorType[0, float]
-
-
-@dataclass
-class DBParametrization(PFBasedParametrization):
-    r"""
-    Corresponds to $\mathcal{O}_{PF} = \mathcal{O}_1 \times \mathcal{O}_2 \times \mathcal{O}_3$, where
-    $\mathcal{O}_1$ is the set of functions from the internal states (no $s_f$)
-    to $\mathbb{R}^+$ (which we parametrize with logs, to avoid the non-negativity constraint),
-    and $\mathcal{O}_2$ is the set of forward probability functions consistent with the DAG.
-    $\mathcal{O}_3$ is the set of backward probability functions consistent with the DAG, or a singleton
-    thereof, if self.logit_PB is a fixed LogitPBEstimator.
-    Useful for the Detailed Balance Loss.
+from gfn.containers import Trajectories, Transitions
+from gfn.gflownet.base import PFBasedGFlowNet
+from gfn.modules import ScalarEstimator
+
+
+class DBGFlowNet(PFBasedGFlowNet):
+    r"""The Detailed Balance GFlowNet.
+
+    Corresponds to $\mathcal{O}_{PF} = \mathcal{O}_1 \times \mathcal{O}_2 \times
+    \mathcal{O}_3$, where $\mathcal{O}_1$ is the set of functions from the internal
+    states (no $s_f$) to $\mathbb{R}^+$ (which we parametrize with logs, to avoid the
+    non-negativity constraint), and $\mathcal{O}_2$ is the set of forward probability
+    functions consistent with the DAG. $\mathcal{O}_3$ is the set of backward
+    probability functions consistent with the DAG, or a singleton thereof, if
+    `self.logit_PB` is a fixed `DiscretePBEstimator`.
+
+    Attributes:
+        logF: a ScalarEstimator instance.
+        on_policy: boolean indicating whether we need to reevaluate the log probs.
+        forward_looking: whether to implement the forward looking GFN loss.
     """
-    logF: LogStateFlowEstimator
 
-
-class DetailedBalance(EdgeDecomposableLoss):
-    def __init__(self, parametrization: DBParametrization, on_policy: bool = False):
-        "If on_policy is True, the log probs stored in the transitions are used."
-        self.parametrization = parametrization
-        self.actions_sampler = DiscreteActionsSampler(parametrization.logit_PF)
-        self.backward_actions_sampler = BackwardDiscreteActionsSampler(
-            parametrization.logit_PB
-        )
-        self.on_policy = on_policy
-
-    def get_scores(self, transitions: Transitions):
+    def __init__(
+        self,
+        logF: ScalarEstimator,
+        forward_looking: bool = False,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+        self.logF = logF
+        self.forward_looking = forward_looking
+        self.env = self.logF.env  # TODO We don't want to store env in here...
+
+    def get_scores(
+        self, transitions: Transitions
+    ) -> Tuple[
+        TT["n_transitions", float],
+        TT["n_transitions", float],
+        TT["n_transitions", float],
+    ]:
+        """Given a batch of transitions, calculate the scores.
+
+        Args:
+            transitions: a batch of transitions.
+
+        Raises:
+            ValueError: when supplied with backward transitions.
+            AssertionError: when log rewards of transitions are None.
+        """
         if transitions.is_backward:
             raise ValueError("Backward transitions are not supported")
         states = transitions.states
         actions = transitions.actions
 
         # uncomment next line for debugging
-        # assert transitions.states.is_sink_state.equal(transitions.actions == -1)
+        # assert transitions.states.is_sink_state.equal(transitions.actions.is_dummy)
 
-        if states.batch_shape != tuple(actions.shape):
+        if states.batch_shape != tuple(actions.batch_shape):
             raise ValueError("Something wrong happening with log_pf evaluations")
         if self.on_policy:
             valid_log_pf_actions = transitions.log_probs
         else:
-            valid_pf_logits = self.actions_sampler.get_logits(states)
-            valid_log_pf_all = valid_pf_logits.log_softmax(dim=-1)
-            valid_log_pf_actions = torch.gather(
-                valid_log_pf_all, dim=-1, index=actions.unsqueeze(-1)
-            ).squeeze(-1)
-
-        valid_log_F_s = self.parametrization.logF(states).squeeze(-1)
+            module_output = self.pf(states)
+            valid_log_pf_actions = self.pf.to_probability_distribution(
+                states, module_output
+            ).log_prob(actions.tensor)
+
+        valid_log_F_s = self.logF(states).squeeze(-1)
+        if self.forward_looking:
+            log_rewards = self.env.log_reward(states)  # RM unsqueeze(-1)
+            valid_log_F_s = valid_log_F_s + log_rewards
 
         preds = valid_log_pf_actions + valid_log_F_s
-
         targets = torch.zeros_like(preds)
 
         # uncomment next line for debugging
         # assert transitions.next_states.is_sink_state.equal(transitions.is_done)
 
         # automatically removes invalid transitions (i.e. s_f -> s_f)
         valid_next_states = transitions.next_states[~transitions.is_done]
-        non_exit_actions = actions[actions != transitions.env.n_actions - 1]
-        valid_pb_logits = self.backward_actions_sampler.get_logits(valid_next_states)
-        valid_log_pb_all = valid_pb_logits.log_softmax(dim=-1)
-        valid_log_pb_actions = torch.gather(
-            valid_log_pb_all, dim=-1, index=non_exit_actions.unsqueeze(-1)
-        ).squeeze(-1)
+        non_exit_actions = actions[~actions.is_exit]
+
+        module_output = self.pb(valid_next_states)
+        valid_log_pb_actions = self.pb.to_probability_distribution(
+            valid_next_states, module_output
+        ).log_prob(non_exit_actions.tensor)
 
         valid_transitions_is_done = transitions.is_done[
             ~transitions.states.is_sink_state
         ]
 
-        valid_log_F_s_next = self.parametrization.logF(valid_next_states).squeeze(-1)
+        valid_log_F_s_next = self.logF(valid_next_states).squeeze(-1)
         targets[~valid_transitions_is_done] = valid_log_pb_actions
         log_pb_actions = targets.clone()
         targets[~valid_transitions_is_done] += valid_log_F_s_next
         assert transitions.log_rewards is not None
         valid_transitions_log_rewards = transitions.log_rewards[
             ~transitions.states.is_sink_state
         ]
@@ -94,54 +106,86 @@
             valid_transitions_is_done
         ]
 
         scores = preds - targets
 
         return (valid_log_pf_actions, log_pb_actions, scores)
 
-    def __call__(self, transitions: Transitions) -> LossTensor:
+    def loss(self, transitions: Transitions) -> TT[0, float]:
+        """Detailed balance loss.
+
+        The detailed balance loss is described in section
+        3.2 of [GFlowNet Foundations](https://arxiv.org/abs/2111.09266)."""
         _, _, scores = self.get_scores(transitions)
         loss = torch.mean(scores**2)
 
         if torch.isnan(loss):
             raise ValueError("loss is nan")
 
         return loss
 
-    def get_modified_scores(self, transitions: Transitions) -> ScoresTensor:
-        "DAG-GFN-style detailed balance, for when all states are connected to the sink"
+    def to_training_samples(self, trajectories: Trajectories) -> Transitions:
+        return trajectories.to_transitions()
+
+
+class ModifiedDBGFlowNet(PFBasedGFlowNet):
+    r"""The Modified Detailed Balance GFlowNet. Only applicable to environments where
+    all states are terminating.
+
+    See Bayesian Structure Learning with Generative Flow Networks
+    https://arxiv.org/abs/2202.13903 for more details.
+    """
+
+    def get_scores(self, transitions: Transitions) -> TT["n_trajectories", torch.float]:
+        """DAG-GFN-style detailed balance, when all states are connected to the sink.
+
+        Raises:
+            ValueError: when backward transitions are supplied (not supported).
+            ValueError: when the computed scores contain `inf`.
+        """
         if transitions.is_backward:
             raise ValueError("Backward transitions are not supported")
+
         mask = ~transitions.next_states.is_sink_state
         states = transitions.states[mask]
         valid_next_states = transitions.next_states[mask]
         actions = transitions.actions[mask]
         all_log_rewards = transitions.all_log_rewards[mask]
-
-        valid_pf_logits = self.actions_sampler.get_logits(states)
-        valid_log_pf_all = valid_pf_logits.log_softmax(dim=-1)
-        valid_log_pf_actions = torch.gather(
-            valid_log_pf_all, dim=-1, index=actions.unsqueeze(-1)
-        ).squeeze(-1)
-        valid_log_pf_s_exit = valid_log_pf_all[:, -1]
+        module_output = self.pf(states)
+        pf_dist = self.pf.to_probability_distribution(states, module_output)
+        if self.on_policy:
+            valid_log_pf_actions = transitions[mask].log_probs
+        else:
+            valid_log_pf_actions = pf_dist.log_prob(actions.tensor)
+        valid_log_pf_s_exit = pf_dist.log_prob(
+            torch.full_like(actions.tensor, actions.__class__.exit_action[0])
+        )
 
         # The following two lines are slightly inefficient, given that most
         # next_states are also states, for which we already did a forward pass.
-        valid_log_pf_s_prime_all = self.actions_sampler.get_logits(
-            valid_next_states
-        ).log_softmax(dim=-1)
-        valid_log_pf_s_prime_exit = valid_log_pf_s_prime_all[:, -1]
-
-        valid_pb_logits = self.backward_actions_sampler.get_logits(valid_next_states)
-        valid_log_pb_all = valid_pb_logits.log_softmax(dim=-1)
-        valid_log_pb_actions = torch.gather(
-            valid_log_pb_all, dim=-1, index=actions.unsqueeze(-1)
-        ).squeeze(-1)
+        module_output = self.pf(valid_next_states)
+        valid_log_pf_s_prime_exit = self.pf.to_probability_distribution(
+            valid_next_states, module_output
+        ).log_prob(torch.full_like(actions.tensor, actions.__class__.exit_action[0]))
+
+        non_exit_actions = actions[~actions.is_exit]
+        module_output = self.pb(valid_next_states)
+        valid_log_pb_actions = self.pb.to_probability_distribution(
+            valid_next_states, module_output
+        ).log_prob(non_exit_actions.tensor)
 
         preds = all_log_rewards[:, 0] + valid_log_pf_actions + valid_log_pf_s_prime_exit
         targets = all_log_rewards[:, 1] + valid_log_pb_actions + valid_log_pf_s_exit
 
         scores = preds - targets
         if torch.any(torch.isinf(scores)):
             raise ValueError("scores contains inf")
 
         return scores
+
+    def loss(self, transitions: Transitions) -> TT[0, float]:
+        """Calculates the modified detailed balance loss."""
+        scores = self.get_scores(transitions)
+        return torch.mean(scores**2)
+
+    def to_training_samples(self, trajectories: Trajectories) -> Transitions:
+        return trajectories.to_transitions()
```

### Comparing `torchgfn-0.2/src/gfn/losses/flow_matching.py` & `torchgfn-1.0.0/src/gfn/gflownet/flow_matching.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,130 @@
-from dataclasses import dataclass
 from typing import Tuple
 
 import torch
-from torchtyping import TensorType
+from torchtyping import TensorType as TT
+
+from gfn.containers import Trajectories
+from gfn.gflownet.base import GFlowNet
+from gfn.modules import DiscretePolicyEstimator
+from gfn.samplers import Sampler
+from gfn.states import DiscreteStates
+
+
+class FMGFlowNet(GFlowNet):
+    r"""Flow Matching GFlowNet, with edge flow estimator.
 
-from gfn.containers.states import States, correct_cast
-from gfn.distributions import EmpiricalTrajectoryDistribution, TrajectoryDistribution
-from gfn.envs import Env
-from gfn.estimators import LogEdgeFlowEstimator
-from gfn.losses.base import Parametrization, StateDecomposableLoss
-from gfn.samplers import DiscreteActionsSampler, TrajectoriesSampler
-
-# Typing
-ScoresTensor = TensorType["n_states", float]
-LossTensor = TensorType[0, float]
-
-
-@dataclass
-class FMParametrization(Parametrization):
-    r"""
     $\mathcal{O}_{edge}$ is the set of functions from the non-terminating edges
     to $\mathbb{R}^+$. Which is equivalent to the set of functions from the internal nodes
     (i.e. without $s_f$) to $(\mathbb{R})^{n_actions}$, without the exit action (No need for
     positivity if we parametrize log-flows).
-    """
-    logF: LogEdgeFlowEstimator
 
-    def Pi(
-        self, env: Env, n_samples: int = 1000, **actions_sampler_kwargs
-    ) -> TrajectoryDistribution:
-        actions_sampler = DiscreteActionsSampler(self.logF, **actions_sampler_kwargs)
-        trajectories_sampler = TrajectoriesSampler(env, actions_sampler)
-        trajectories = trajectories_sampler.sample_trajectories(
-            n_trajectories=n_samples
-        )
-        return EmpiricalTrajectoryDistribution(trajectories)
+    The loss is described in section
+    3.2 of [GFlowNet Foundations](https://arxiv.org/abs/2111.09266).
 
+    Attributes:
+        logF: LogEdgeFlowEstimator
+        alpha: weight for the reward matching loss.
+    """
 
-class FlowMatching(StateDecomposableLoss):
-    def __init__(self, parametrization: FMParametrization, alpha=1.0) -> None:
-        "alpha is the weight of the reward matching loss"
-        self.parametrization = parametrization
-        self.env = parametrization.logF.env
-        self.alpha = alpha
+    def __init__(self, logF: DiscretePolicyEstimator, alpha: float = 1.0):
+        super().__init__()
+        assert not logF.greedy_eps
 
-    def flow_matching_loss(self, states: States) -> ScoresTensor:
-        """
-        Compute the FM for the given states, defined as the log-sum incoming flows minus log-sum outgoing flows.
-        The states should not include s0. The batch shape should be (n_states,).
+        self.logF = logF
+        self.alpha = alpha
+        self.env = self.logF.env
+        if not self.env.is_discrete:
+            raise NotImplementedError(
+                "Flow Matching GFlowNet only supports discrete environments for now."
+            )
 
-        As of now, only discrete environments are handled.
+    def sample_trajectories(self, n_samples: int = 1000) -> Trajectories:
+        sampler = Sampler(estimator=self.logF)
+        trajectories = sampler.sample_trajectories(n_trajectories=n_samples)
+        return trajectories
+
+    def flow_matching_loss(
+        self, states: DiscreteStates
+    ) -> TT["n_trajectories", torch.float]:
+        """Computes the FM for the provided states.
+
+        The Flow Matching loss is defined as the log-sum incoming flows minus log-sum
+        outgoing flows. The states should not include $s_0$. The batch shape should be
+        `(n_states,)`. As of now, only discrete environments are handled.
+
+        Raises:
+            AssertionError: If the batch shape is not linear.
+            AssertionError: If any state is at $s_0$.
         """
 
         assert len(states.batch_shape) == 1
         assert not torch.any(states.is_initial_state)
 
-        states.forward_masks, states.backward_masks = correct_cast(
-            states.forward_masks, states.backward_masks
-        )
-
         incoming_log_flows = torch.full_like(
             states.backward_masks, -float("inf"), dtype=torch.float
         )
         outgoing_log_flows = torch.full_like(
             states.forward_masks, -float("inf"), dtype=torch.float
         )
 
         for action_idx in range(self.env.n_actions - 1):
-            # TODO: can this be done in a vectorized way? Maybe by "repeating" the states and creating a big actions tensor?
             valid_backward_mask = states.backward_masks[:, action_idx]
             valid_forward_mask = states.forward_masks[:, action_idx]
             valid_backward_states = states[valid_backward_mask]
             valid_forward_states = states[valid_forward_mask]
-            _, valid_backward_states.backward_masks = correct_cast(
-                valid_backward_states.forward_masks,
-                valid_backward_states.backward_masks,
-            )
+
             backward_actions = torch.full_like(
                 valid_backward_states.backward_masks[:, 0], action_idx, dtype=torch.long
-            )
+            ).unsqueeze(-1)
+            backward_actions = self.env.Actions(backward_actions)
 
             valid_backward_states_parents = self.env.backward_step(
                 valid_backward_states, backward_actions
             )
 
-            incoming_log_flows[
-                valid_backward_mask, action_idx
-            ] = self.parametrization.logF(valid_backward_states_parents)[:, action_idx]
-            outgoing_log_flows[
-                valid_forward_mask, action_idx
-            ] = self.parametrization.logF(valid_forward_states)[:, action_idx]
+            incoming_log_flows[valid_backward_mask, action_idx] = self.logF(
+                valid_backward_states_parents
+            )[:, action_idx]
+
+            outgoing_log_flows[valid_forward_mask, action_idx] = self.logF(
+                valid_forward_states
+            )[:, action_idx]
 
         # Now the exit action
         valid_forward_mask = states.forward_masks[:, -1]
-        outgoing_log_flows[valid_forward_mask, -1] = self.parametrization.logF(
+        outgoing_log_flows[valid_forward_mask, -1] = self.logF(
             states[valid_forward_mask]
         )[:, -1]
 
         log_incoming_flows = torch.logsumexp(incoming_log_flows, dim=-1)
         log_outgoing_flows = torch.logsumexp(outgoing_log_flows, dim=-1)
 
         return (log_incoming_flows - log_outgoing_flows).pow(2).mean()
 
-    def reward_matching_loss(self, terminating_states: States) -> LossTensor:
+    def reward_matching_loss(self, terminating_states: DiscreteStates) -> TT[0, float]:
+        """Calculates the reward matching loss from the terminating states."""
         assert terminating_states.log_rewards is not None
-        log_edge_flows = self.parametrization.logF(terminating_states)
+        log_edge_flows = self.logF(terminating_states)
+
+        # Handle the boundary condition (for all x, F(X->S_f) = R(x)).
         terminating_log_edge_flows = log_edge_flows[:, -1]
         log_rewards = terminating_states.log_rewards
         return (terminating_log_edge_flows - log_rewards).pow(2).mean()
 
-    def __call__(self, states_tuple: Tuple[States, States]) -> LossTensor:
+    def loss(self, states_tuple: Tuple[DiscreteStates, DiscreteStates]) -> TT[0, float]:
+        """Given a batch of non-terminal and terminal states, compute a loss.
+
+        Unlike the GFlowNets Foundations paper, we allow more flexibility by passing a
+        tuple of states, the first one being the internal states of the trajectories
+        (i.e. non-terminal states), and the second one being the terminal states of the
+        trajectories."""
         intermediary_states, terminating_states = states_tuple
         fm_loss = self.flow_matching_loss(intermediary_states)
         rm_loss = self.reward_matching_loss(terminating_states)
         return fm_loss + self.alpha * rm_loss
+
+    def to_training_samples(
+        self, trajectories: Trajectories
+    ) -> tuple[DiscreteStates, DiscreteStates]:
+        """Converts a batch of trajectories into a batch of training samples."""
+        return trajectories.to_non_initial_intermediary_and_terminating_states()
```

### Comparing `torchgfn-0.2/src/gfn/losses/sub_trajectory_balance.py` & `torchgfn-1.0.0/src/gfn/gflownet/sub_trajectory_balance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,133 +1,138 @@
-from dataclasses import dataclass
 from typing import List, Literal, Tuple
 
 import torch
-from torchtyping import TensorType
+from torchtyping import TensorType as TT
 
 from gfn.containers import Trajectories
-from gfn.estimators import LogStateFlowEstimator
-from gfn.losses.base import PFBasedParametrization, TrajectoryDecomposableLoss
-from gfn.samplers.actions_samplers import (
-    BackwardDiscreteActionsSampler,
-    DiscreteActionsSampler,
-)
-
-# Typing
-ScoresTensor = TensorType[-1, float]
-LossTensor = TensorType[0, float]
-LogPTrajectoriesTensor = TensorType["max_length", "n_trajectories", float]
-
-
-@dataclass
-class SubTBParametrization(PFBasedParametrization):
-    r"""
-    Exactly the same as DBParametrization
-    """
-    logF: LogStateFlowEstimator
+from gfn.gflownet.base import PFBasedGFlowNet, TrajectoryBasedGFlowNet
+from gfn.modules import ScalarEstimator
+
 
+class SubTBGFlowNet(TrajectoryBasedGFlowNet):
+    r"""GFlowNet for the Sub Trajectory Balance Loss.
+
+    This method is described in [Learning GFlowNets from partial episodes
+    for improved convergence and stability](https://arxiv.org/abs/2209.12782).
+
+    Attributes:
+        logF: a LogStateFlowEstimator instance.
+        weighting: sub-trajectories weighting scheme.
+            - "DB": Considers all one-step transitions of each trajectory in the
+                batch and weighs them equally (regardless of the length of
+                trajectory). Should be equivalent to DetailedBalance loss.
+            - "ModifiedDB": Considers all one-step transitions of each trajectory
+                in the batch and weighs them inversely proportional to the
+                trajectory length. This ensures that the loss is not dominated by
+                long trajectories. Each trajectory contributes equally to the loss.
+            - "TB": Considers only the full trajectory. Should be equivalent to
+                TrajectoryBalance loss.
+            - "equal_within": Each sub-trajectory of each trajectory is weighed
+                equally within the trajectory. Then each trajectory is weighed
+                equally within the batch.
+            - "equal": Each sub-trajectory of each trajectory is weighed equally
+                within the set of all sub-trajectories.
+            - "geometric_within": Each sub-trajectory of each trajectory is weighed
+                proportionally to (lamda ** len(sub_trajectory)), within each
+                trajectory. THIS CORRESPONDS TO THE ONE IN THE PAPER.
+            - "geometric": Each sub-trajectory of each trajectory is weighed
+                proportionally to (lamda ** len(sub_trajectory)), within the set of
+                all sub-trajectories.
+        lamda: discount factor for longer trajectories.
+        log_reward_clip_min: minimum value for log rewards.
+    """
 
-class SubTrajectoryBalance(TrajectoryDecomposableLoss):
     def __init__(
         self,
-        parametrization: SubTBParametrization,
-        log_reward_clip_min: float = -12,
-        weighing: Literal[
+        logF: ScalarEstimator,
+        weighting: Literal[
             "DB",
             "ModifiedDB",
             "TB",
             "geometric",
             "equal",
             "geometric_within",
             "equal_within",
-        ] = "geometric",
+        ] = "geometric_within",
         lamda: float = 0.9,
-        on_policy: bool = False,
+        log_reward_clip_min: float = -12,  # roughly log(1e-5)
+        forward_looking: bool = False,
+        **kwargs,
     ):
-        """
-        :param parametrization: parametrization of the model
-        :param log_reward_clip_min: minimum value of the log-reward. Log-Rewards lower than this value will be clipped to this value. Defaults to -12 (roughly log(1e-5)).
-        :param weighing: how to weigh the different sub-trajectories of each trajectory.
-            - "DB": Considers all one-step transitions of each trajectory in the batch and weighs them equally (regardless of the length of trajectory).
-                    Should be equivalent to DetailedBalance loss.
-            - "ModifiedDB": Considers all one-step transitions of each trajectory in the batch and weighs them inversely proportional to the trajectory length.
-                    This ensures that the loss is not dominated by long trajectories. Each trajectory contributes equally to the loss.
-            - "TB": Considers only the full trajectory. Should be equivalent to TrajectoryBalance loss.
-            - "equal_within": Each sub-trajectory of each trajectory is weighed equally within the trajectory. Then each trajectory is weighed equally within the batch.
-            - "equal": Each sub-trajectory of each trajectory is weighed equally within the set of all sub-trajectories.
-            - "geometric_within": Each sub-trajectory of each trajectory is weighed proportionally to (lamda ** len(sub_trajectory)), within each trajectory.
-            - "geometric": Each sub-trajectory of each trajectory is weighed proportionally to (lamda ** len(sub_trajectory)), within the set of all sub-trajectories.
-        :param lamda: parameter for geometric weighing
-        :param on_policy: whether the loss is computed on-policy (in which case the log probs stored in the trajectories are used) or off-policy
-        """
-        # Lamda is a discount factor for longer trajectories. The part of the loss
-        # corresponding to sub-trajectories of length i is multiplied by lamda^i
-        # where an edge is of length 1. As lamda approaches 1, each loss becomes equally weighted.
-        self.parametrization = parametrization
-        self.log_reward_clip_min = log_reward_clip_min
-        self.actions_sampler = DiscreteActionsSampler(parametrization.logit_PF)
-        self.backward_actions_sampler = BackwardDiscreteActionsSampler(
-            parametrization.logit_PB
-        )
-        self.weighing = weighing
+        super().__init__(**kwargs)
+        self.logF = logF
+        self.weighting = weighting
         self.lamda = lamda
-        self.on_policy = on_policy
+        self.log_reward_clip_min = log_reward_clip_min
+        self.forward_looking = forward_looking
 
     def cumulative_logprobs(
         self,
         trajectories: Trajectories,
-        log_p_trajectories: LogPTrajectoriesTensor,
-    ) -> LogPTrajectoriesTensor:
-        """
-        :param trajectories: trajectories
-        :param log_p_trajectories: log probabilities of each transition in each trajectory
-        :return: cumulative sum of log probabilities of each trajectory
+        log_p_trajectories: TT["max_length", "n_trajectories", torch.float],
+    ) -> TT["max_length", "n_trajectories", torch.float]:
+        """Calculates the cumulative log probabilities for all trajectories.
+
+        Args:
+            trajectories: a batch of trajectories.
+            log_p_trajectories: log probabilities of each transition in each trajectory.
+
+        Returns: cumulative sum of log probabilities of each trajectory.
         """
         return torch.cat(
             (
                 torch.zeros(
                     1, trajectories.n_trajectories, device=log_p_trajectories.device
                 ),
                 log_p_trajectories.cumsum(dim=0),
             ),
             dim=0,
         )
 
     def get_scores(
         self, trajectories: Trajectories
-    ) -> Tuple[List[ScoresTensor], List[ScoresTensor]]:
-        """
-        Returns two elements:
-        - A list of tensors, each of which representing the scores of all sub-trajectories of length k, for k in [1, ..., trajectories.max_length].
-            where the score of a sub-trajectory tau is log P_F(tau) + log F(tau_0) - log P_B(tau) - log F(tau_{-1}). The shape of the k-th tensor
-            is (trajectories.max_length - k + 1, trajectories.n_trajectories), k starting from 1.
-        - A list of tensors representing what should be masked out in the each element of the first list, given that not all sub-trajectories
-            of length k exist for each trajectory. The entries of those tensors are True if the corresponding sub-trajectory does not exist.
+    ) -> Tuple[List[TT[0, float]], List[TT[0, float]]]:
+        """Scores all submitted trajectories.
+
+        Returns:
+            - A list of tensors, each of which representing the scores of all
+                sub-trajectories of length k, for k in `[1, ...,
+                trajectories.max_length]`, where the score of a sub-trajectory tau is
+                $log P_F(tau) + log F(tau_0) - log P_B(tau) - log F(tau_{-1})$. The
+                shape of the k-th tensor is `(trajectories.max_length - k + 1,
+                trajectories.n_trajectories)`, k starting from 1.
+            - A list of tensors representing what should be masked out in the each
+                element of the first list, given that not all sub-trajectories
+                of length k exist for each trajectory. The entries of those tensors are
+                True if the corresponding sub-trajectory does not exist.
         """
         log_pf_trajectories, log_pb_trajectories = self.get_pfs_and_pbs(
-            trajectories, fill_value=-float("inf"), no_pf=self.on_policy
+            trajectories, fill_value=-float("inf")
         )
-        if self.on_policy:
-            log_pf_trajectories = trajectories.log_probs
 
         log_pf_trajectories_cum = self.cumulative_logprobs(
             trajectories, log_pf_trajectories
         )
         log_pb_trajectories_cum = self.cumulative_logprobs(
             trajectories, log_pb_trajectories
         )
 
         states = trajectories.states
         log_state_flows = torch.full_like(log_pf_trajectories, fill_value=-float("inf"))
         mask = ~states.is_sink_state
         valid_states = states[mask]
-        log_state_flows[mask[:-1]] = self.parametrization.logF(valid_states).squeeze(-1)
+
+        log_F = self.logF(valid_states).squeeze(-1)
+        if self.forward_looking:
+            log_rewards = self.logF.env.log_reward(states).unsqueeze(-1)
+            log_F = log_F + log_rewards
+        log_state_flows[mask[:-1]] = log_F
 
         sink_states_mask = log_state_flows == -float("inf")
-        is_terminal_mask = trajectories.actions == trajectories.env.n_actions - 1
+        is_terminal_mask = trajectories.actions.is_exit
         full_mask = sink_states_mask | is_terminal_mask
 
         flattening_masks = []
         scores = []
         for i in range(1, 1 + trajectories.max_length):
             current_log_state_flows = (
                 log_state_flows if i == 1 else log_state_flows[: -(i - 1)]
@@ -136,15 +141,19 @@
             preds = (
                 log_pf_trajectories_cum[i:]
                 - log_pf_trajectories_cum[:-i]
                 + current_log_state_flows
             )
 
             targets = torch.full_like(preds, fill_value=-float("inf"))
-            targets.T[is_terminal_mask[i - 1 :].T] = trajectories.log_rewards[trajectories.when_is_done >= i].clamp_min(self.log_reward_clip_min)  # type: ignore
+            assert trajectories.log_rewards is not None
+            log_rewards = trajectories.log_rewards[
+                trajectories.when_is_done >= i
+            ].clamp_min(self.log_reward_clip_min)
+            targets.T[is_terminal_mask[i - 1 :].T] = log_rewards
 
             # For now, the targets contain the log-rewards of the ending sub trajectories
             # We need to add to that the log-probabilities of the backward actions up-to
             # the sub-trajectory's terminating state
             if i > 1:
                 targets[is_terminal_mask[i - 1 :]] += (
                     log_pb_trajectories_cum[i - 1 :] - log_pb_trajectories_cum[: -i + 1]
@@ -175,130 +184,116 @@
             scores.append(preds - targets)
 
         return (
             scores,
             flattening_masks,
         )
 
-    def __call__(self, trajectories: Trajectories) -> LossTensor:
-        (
-            scores,
-            flattening_masks,
-        ) = self.get_scores(trajectories)
-
+    def loss(self, trajectories: Trajectories) -> TT[0, float]:
+        # Get all scores and masks from the trajectories.
+        scores, flattening_masks = self.get_scores(trajectories)
         flattening_mask = torch.cat(flattening_masks)
         all_scores = torch.cat(scores, 0)
 
-        # all_scores is a tensor of shape (max_length * (max_length + 1) / 2, n_trajectories)
-        n_rows = int(trajectories.max_length * (1 + trajectories.max_length) / 2)
+        # Used only to keep the following calculations clean.
+        L = self.lamda
+        max_len = trajectories.max_length
+        is_done = trajectories.when_is_done
+
+        # all_scores is a tensor of shape (max_len * (max_leng + 1) / 2, n_trajectories)
+        n_rows = int(max_len * (1 + max_len) / 2)
 
-        if self.weighing == "equal_within":
+        if self.weighting == "equal_within":
             # the following tensor represents the inverse of how many sub-trajectories there are in each trajectory
-            contributions = 2.0 / (
-                trajectories.when_is_done * (trajectories.when_is_done + 1)
-            )
-            contributions = contributions / len(trajectories)
-            # if we repeat the previous tensor, we get a tensor of shape (max_length * (max_length + 1) / 2, n_trajectories)
-            # that we can multiply with all_scores to get a loss where each sub-trajectory is weighted equally within each trajectory
+            contributions = 2.0 / (is_done * (is_done + 1)) / len(trajectories)
+
+            # if we repeat the previous tensor, we get a tensor of shape
+            # (max_len * (max_len + 1) / 2, n_trajectories) that we can multiply with
+            # all_scores to get a loss where each sub-trajectory is weighted equally
+            # within each trajectory.
             contributions = contributions.repeat(n_rows, 1)
-        elif self.weighing == "equal":
-            n_sub_trajectories = int(
-                (trajectories.when_is_done * (trajectories.when_is_done + 1) / 2)
-                .sum()
-                .item()
-            )
+
+        elif self.weighting == "equal":
+            n_sub_trajectories = int((is_done * (is_done + 1) / 2).sum().item())
             contributions = torch.ones(n_rows, len(trajectories)) / n_sub_trajectories
-        elif self.weighing == "TB":
+
+        elif self.weighting == "TB":
             # Each trajectory contributes one element to the loss, equally weighted
             contributions = torch.zeros_like(all_scores)
             indices = (
-                trajectories.max_length * (trajectories.when_is_done - 1)
-                - (trajectories.when_is_done - 1) * (trajectories.when_is_done - 2) / 2
+                max_len * (is_done - 1) - (is_done - 1) * (is_done - 2) / 2
             ).long()
             contributions.scatter_(0, indices.unsqueeze(0), 1)
             contributions = contributions / len(trajectories)
-        elif self.weighing == "DB":
+
+        elif self.weighting == "DB":
             # Longer trajectories contribute more to the loss
             return scores[0][~flattening_masks[0]].pow(2).mean()
-        elif self.weighing == "ModifiedDB":
-            # The following tensor represents the inverse of how many transitions there are in each trajectory
-            contributions = 1.0 / trajectories.when_is_done
-            contributions = contributions / len(trajectories)
-            contributions = contributions.repeat(trajectories.max_length, 1)
+
+        elif self.weighting == "ModifiedDB":
+            # The following tensor represents the inverse of how many transitions
+            # there are in each trajectory.
+            contributions = (1.0 / is_done / len(trajectories)).repeat(max_len, 1)
             contributions = torch.cat(
                 (
                     contributions,
                     torch.zeros(
-                        (n_rows - trajectories.max_length, len(trajectories)),
+                        (n_rows - max_len, len(trajectories)),
                         device=contributions.device,
                     ),
                 ),
                 0,
             )
 
-        elif self.weighing == "geometric_within":
-            # the following tensor represents the weights given to each possible sub-trajectory length
-            contributions = (
-                self.lamda ** torch.arange(trajectories.max_length).double()
-            ).float()
+        elif self.weighting == "geometric_within":
+            # The following tensor represents the weights given to each possible
+            # sub-trajectory length.
+            contributions = (L ** torch.arange(max_len).double()).float()
             contributions = contributions.unsqueeze(-1).repeat(1, len(trajectories))
-
             contributions = contributions.repeat_interleave(
-                torch.arange(trajectories.max_length, 0, -1),
+                torch.arange(max_len, 0, -1),
                 dim=0,
-                output_size=int(
-                    trajectories.max_length * (trajectories.max_length + 1) / 2
-                ),
+                output_size=int(max_len * (max_len + 1) / 2),
             )
-            r"""
-            Now we need to divide each column by n + (n-1) lambda +...+ 1*lambda^{n-1}
-            where n is the length of the trajectory corresponding to that column
-            We can do it the ugly way, or using the cool identity:
-            https://www.wolframalpha.com/input?i=sum%28%28n-i%29+*+lambda+%5Ei%2C+i%3D0..n%29
-            """
-            per_trajectory_denominator = (
+
+            # Now we need to divide each column by n + (n-1) lambda +...+ 1*lambda^{n-1}
+            # where n is the length of the trajectory corresponding to that column
+            # We can do it the ugly way, or using the cool identity:
+            # https://www.wolframalpha.com/input?i=sum%28%28n-i%29+*+lambda+%5Ei%2C+i%3D0..n%29
+            per_trajectory_denom = (
                 1.0
-                / (1 - self.lamda) ** 2
-                * (
-                    self.lamda * (self.lamda ** trajectories.when_is_done.double() - 1)
-                    + (1 - self.lamda) * trajectories.when_is_done.double()
-                )
+                / (1 - L) ** 2
+                * (L * (L ** is_done.double() - 1) + (1 - L) * is_done.double())
             ).float()
-            contributions = contributions / per_trajectory_denominator
-            contributions = contributions / len(trajectories)
+            contributions = contributions / per_trajectory_denom / len(trajectories)
 
-        elif self.weighing == "geometric":
-            # The position i of the following 1D tensor represents the number of sub-trajectories of length i in the batch
+        elif self.weighting == "geometric":
+            # The position i of the following 1D tensor represents the number of sub-
+            # trajectories of length i in the batch.
             # n_sub_trajectories = torch.maximum(
             #     trajectories.when_is_done - torch.arange(3).unsqueeze(-1),
             #     torch.tensor(0),
             # ).sum(1)
 
-            # The following tensor's k-th entry represents the mean of all losses of sub-trajectories of length k
+            # The following tensor's k-th entry represents the mean of all losses of
+            # sub-trajectories of length k.
             per_length_losses = torch.stack(
                 [
                     scores[~flattening_mask].pow(2).mean()
                     for scores, flattening_mask in zip(scores, flattening_masks)
                 ]
             )
-            ld = self.lamda
-            weights = (
-                (1 - ld)
-                / (1 - ld**trajectories.max_length)
-                * (
-                    ld
-                    ** torch.arange(
-                        trajectories.max_length, device=per_length_losses.device
-                    )
-                )
+            ratio = (1 - L) / (1 - L**max_len)
+            weights = ratio * (
+                L ** torch.arange(max_len, device=per_length_losses.device)
             )
             assert (weights.sum() - 1.0).abs() < 1e-5, f"{weights.sum()}"
             return (per_length_losses * weights).sum()
         else:
-            raise ValueError(f"Unknown weighing method {self.weighing}")
+            raise ValueError(f"Unknown weighting method {self.weighting}")
 
         flat_contributions = contributions[~flattening_mask]
         assert (
             flat_contributions.sum() - 1.0
         ).abs() < 1e-5, f"{flat_contributions.sum()}"
         losses = flat_contributions * all_scores[~flattening_mask].pow(2)
         return losses.sum()
```

### Comparing `torchgfn-0.2/PKG-INFO` & `torchgfn-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: torchgfn
-Version: 0.2
+Version: 1.0.0
 Summary: A torch implementation of GFlowNets
 License: MIT
 Author: Salem Lahou
 Author-email: salemlahlou9@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: scripts
 Requires-Dist: black (==22.3.0) ; extra == "dev" or extra == "all"
 Requires-Dist: einops (>=0.6.1)
-Requires-Dist: gymnasium (>=0.28.1)
+Requires-Dist: gitmopy ; extra == "dev"
 Requires-Dist: myst-parser ; extra == "dev" or extra == "all"
 Requires-Dist: numpy (>=1.21.2)
 Requires-Dist: pre-commit ; extra == "dev" or extra == "all"
 Requires-Dist: pytest ; extra == "dev" or extra == "all"
 Requires-Dist: renku-sphinx-theme ; extra == "dev" or extra == "all"
-Requires-Dist: simple-parsing (==0.0.20) ; extra == "scripts" or extra == "all"
+Requires-Dist: scikit-learn ; extra == "scripts" or extra == "all"
+Requires-Dist: scipy ; extra == "scripts" or extra == "all"
 Requires-Dist: sphinx ; extra == "dev" or extra == "all"
 Requires-Dist: sphinx-autoapi ; extra == "dev" or extra == "all"
 Requires-Dist: sphinx-math-dollar ; extra == "dev" or extra == "all"
 Requires-Dist: sphinx_rtd_theme ; extra == "dev" or extra == "all"
 Requires-Dist: torch (>=1.9.0)
 Requires-Dist: torchtyping (>=0.1.4)
 Requires-Dist: tox ; extra == "dev" or extra == "all"
@@ -34,32 +36,32 @@
 Requires-Dist: wandb ; extra == "scripts" or extra == "all"
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a>
 	    <img src='https://img.shields.io/badge/python-3.10%2B-blueviolet' alt='Python' />
 	</a>
-	<a href='https://gfn.readthedocs.io/en/latest/?badge=latest'>
-    	<img src='https://readthedocs.org/projects/gfn/badge/?version=latest' alt='Documentation Status' />
+	<a href='https://torchgfn.readthedocs.io/en/latest/?badge=latest'>
+    	<img src='https://readthedocs.org/projects/torchgfn/badge/?version=latest' alt='Documentation Status' />
 	</a>
     <a>
 	    <img src='https://img.shields.io/badge/code%20style-black-black' />
 	</a>
 </p>
 
 </p>
 <p align="center">
-  <a href="https://gfn.readthedocs.io/en/latest/">Documentation</a> ~ <a href="https://github.com/saleml/gfn">Code</a>
+  <a href="https://torchgfn.readthedocs.io/en/latest/">Documentation</a> ~ <a href="https://github.com/saleml/torchgfn">Code</a> ~ <a href="https://arxiv.org/abs/2305.14594">Paper</a>
 </p>
 
-# gfn: a Python package for GFlowNets
-
+# torchgfn: a Python package for GFlowNets
 
+<p align="center"> Please cite <a href="https://arxiv.org/abs/2305.14594">this paper</a> if you are using the library for your research </p>
 
-## Installing the packages
+## Installing the package
 
 The codebase requires python >= 3.10
 
 To install the latest stable version:
 
 ```bash
 pip install torchgfn
@@ -70,175 +72,169 @@
 ```bash
 pip install torchgfn[scripts]
 ```
 
 To install the cutting edge version (from the `main` branch):
 
 ```bash
-git clone https://github.com/saleml/gfn.git
-conda create -n gfn python=3.11
+git clone https://github.com/saleml/torchgfn.git
+conda create -n gfn python=3.10
 conda activate gfn
-cd gfn
+cd torchgfn
 pip install .
 ```
 
 
 ## About this repo
 
-This repo serves the purpose of fast prototyping [GFlowNet](https://arxiv.org/abs/2111.09266) related algorithms. It decouples the environment definition, the sampling process, and the parametrization used for the GFN loss.
+This repo serves the purpose of fast prototyping [GFlowNet](https://arxiv.org/abs/2111.09266) related algorithms. It decouples the environment definition, the sampling process, and the parametrization of the function approximators used to calculate the GFN loss.
 
-An example script is provided [here](https://github.com/saleml/gfn/blob/master/scripts/train.py). To run the code, use one of the following:
+Example scripts and notebooks are provided [here](https://github.com/saleml/torchgfn/tree/master/tutorials/).
 
-```bash
-python train.py --env hypergrid --env.ndim 4 --env.height 8 --n_iterations 100000 --loss trajectory-balance
-python train.py --env discrete-ebm --env.ndim 4 --env.alpha 0.5 --n_iterations 10000 --batch_size 64 --sampler.temperature 2.
-python train.py --env hypergrid --env.ndim 2 --env.height 64 --n_iterations 100000 --loss detailed-balance --logit_PB.module_name Uniform --optim adam --optim.lr 1e-3 --batch_size 64
-python train.py --env hypergrid --env.ndim 4 --env.height 8 --env.R0 0.01 --loss flowmatching --optim adam --optim.lr 1e-4
-```
 
-### Example, in a few lines
+### Standalone example
 
-(⬇️ This example require the [`tqdm`](https://github.com/tqdm/tqdm) package to run. `pip install tqdm` or install all extra requirements with `pip install .[scripts]`)
+This example, which shows how to use the library for a simple discrete environment, requires [`tqdm`](https://github.com/tqdm/tqdm) package to run. Use `pip install tqdm` or install all extra requirements with `pip install .[scripts]` or `pip install torchgfn[scripts]`.
 
 ```python
 import torch
 from tqdm import tqdm
 
-from gfn import LogitPBEstimator, LogitPFEstimator, LogZEstimator
-from gfn.envs import HyperGrid
-from gfn.losses import TBParametrization, TrajectoryBalance
-from gfn.samplers import DiscreteActionsSampler, TrajectoriesSampler
+from gfn.gflownet import TBGFlowNet
+from gfn.gym import HyperGrid
+from gfn.modules import DiscretePolicyEstimator
+from gfn.samplers import Sampler
+from gfn.utils import NeuralNet
 
 if __name__ == "__main__":
 
     env = HyperGrid(ndim=4, height=8, R0=0.01)  # Grid of size 8x8x8x8
 
-    logit_PF = LogitPFEstimator(env=env, module_name="NeuralNet")
-    logit_PB = LogitPBEstimator(
-        env=env,
-        module_name="NeuralNet",
-        torso=logit_PF.module.torso,  # To share parameters between PF and PB
+    module_PF = NeuralNet(
+        input_dim=env.preprocessor.output_dim,
+        output_dim=env.n_actions
     )
-    logZ = LogZEstimator(torch.tensor(0.0))
+    module_PB = NeuralNet(
+        input_dim=env.preprocessor.output_dim,
+        output_dim=env.n_actions - 1,
+        torso=module_PF.torso
+    )
+
+    pf_estimator = DiscretePolicyEstimator(env, module_PF, forward=True)
+    pb_estimator = DiscretePolicyEstimator(env, module_PB, forward=False)
 
-    parametrization = TBParametrization(logit_PF, logit_PB, logZ)
+    gfn = TBGFlowNet(init_logZ=0., pf=pf_estimator, pb=pb_estimator)
 
-    actions_sampler = DiscreteActionsSampler(estimator=logit_PF)
-    trajectories_sampler = TrajectoriesSampler(env=env, actions_sampler=actions_sampler)
+    sampler = Sampler(estimator=pf_estimator))
 
-    loss_fn = TrajectoryBalance(parametrization=parametrization)
+    # Policy parameters have their own LR.
+    non_logz_params = [v for k, v in dict(gfn.named_parameters()).items() if k != "logZ"]
+    optimizer = torch.optim.Adam(non_logz_params, lr=1e-3)
 
-    params = [
-        {
-            "params": [
-                val for key, val in parametrization.parameters.items() if "logZ" not in key
-            ],
-            "lr": 0.001,
-        },
-        {"params": [val for key, val in parametrization.parameters.items() if "logZ" in key], "lr": 0.1},
-    ]
-    optimizer = torch.optim.Adam(params)
+    # Log Z gets dedicated learning rate (typically higher).
+    logz_params = [dict(gfn.named_parameters())["logZ"]]
+    optimizer.add_param_group({"params": logz_params, "lr": 1e-2})
 
     for i in (pbar := tqdm(range(1000))):
-        trajectories = trajectories_sampler.sample(n_trajectories=16)
+        trajectories = sampler.sample_trajectories(n_trajectories=16)
         optimizer.zero_grad()
-        loss = loss_fn(trajectories)
+        loss = gfn.loss(trajectories)
         loss.backward()
         optimizer.step()
         if i % 25 == 0:
             pbar.set_postfix({"loss": loss.item()})
-
 ```
 
 ## Contributing
 
 Before the first commit:
 
 ```bash
-pip install .[dev]
+pip install -e .[dev,scripts]
 pre-commit install
 pre-commit run --all-files
 ```
 
 Run `pre-commit` after staging, and before committing. Make sure all the tests pass (By running `pytest`).
 The codebase uses `black` formatter.
 
 To make the docs locally:
+
 ```bash
 cd docs
 make html
 open build/html/index.html
 ```
 
 ## Details about the codebase
 
 ### Defining an environment
 
-A pointed DAG environment (or GFN environment, or environment for short) is a representation for the pointed DAG. The abstract class [Env](https://github.com/saleml/gfn/blob/master/src/gfn/envs/env.py) specifies the requirements for a valid environment definition. To obtain such a representation, the environment needs to specify the following attributes, properties, or methods:
+See [here](https://github.com/saleml/torchgfn/tree/master/tutorials/ENV.md)
+
+### States
+
+States are the primitive building blocks for GFlowNet objects such as transitions and trajectories, on which losses operate.
+
+An abstract `States` class is provided. But for each environment, a `States` subclass is needed. A `States` object
+is a collection of multiple states (nodes of the DAG). A tensor representation of the states is required for batching. If a state is represented with a tensor of shape `(*state_shape)`, a batch of states is represented with a `States` object, with the attribute `tensor` of shape `(*batch_shape, *state_shape)`. Other
+representations are possible (e.g. a state as a string, a `numpy` array, a graph, etc...), but these representations cannot be batched, unless the user specifies a function that transforms these raw states to tensors.
 
-- The `action_space`. Which should be a `gymnasium.spaces.Discrete` object for discrete environments. The last action should correspond to the exit action.
-- The initial state `s_0`, as a `torch.Tensor` of arbitrary dimension.
-- (Optional) The sink state `s_f`, as a `torch.Tensor` of the same shape as `s_0`, used to represent complete trajectories only (within a batch of trajectories of different lengths), and never processed by any model. If not specified, it is set to `torch.full_like(s_0, -float('inf'))`.
-- The method `make_States_class` that creates a subclass of [States](https://github.com/saleml/gfn/blob/master/src/gfn/containers/states.py). The instances of the resulting class should represent a batch of states of arbitrary shape, which is useful to define a trajectory, or a batch of trajectories. `s_0` and `s_f`, along with a tuple called `state_shape` should be defined as class variables, and the subclass (of `States`) should implement masking methods, that specify which actions are possible, in a discrete environment.
-- The methods `maskless_step` and `maskless_backward_step` that specify how an action changes a state (going forward and backward). These functions do not need to handle masking, checking whether actions are allowed, checking whether a state is the sink state, etc... These checks are handled in `Env.step` and `Env.backward_step`
-- The `log_reward` function that assigns a nonnegative reward to every terminating state (i.e. state with all $s_f$ as a child in the DAG). If `log_reward` is not implemented, `reward` needs to be.
+The `batch_shape` attribute is required to keep track of the batch dimension. A trajectory can be represented by a States object with `batch_shape = (n_states,)`. Multiple trajectories can be represented by a States object with `batch_shape = (n_states, n_trajectories)`.
 
-If the states (as represented in the `States` class) need to be transformed to another format before being processed (by neural networks for example), then the environment should define a `preprocessor` attribute, which should be an instance of the [base preprocessor class](https://github.com/saleml/gfn/blob/master/src/gfn/envs/preprocessors/base.py). If no preprocessor is defined, the states are used as is (actually transformed using  [`IdentityPreprocessor`](https://github.com/saleml/gfn/blob/master/src/gfn/envs/preprocessors/base.py), which transforms the state tensors to `FloatTensor`s). Implementing your own preprocessor requires defining the `preprocess` function, and the `output_shape` attribute, which is a tuple representing the shape of *one* preprocessed state.
+Because multiple trajectories can have different lengths, batching requires appending a dummy tensor to trajectories that are shorter than the longest trajectory. The dummy state is the $s_f$ attribute of the environment (e.g. `[-1, ..., -1]`, or `[-inf, ..., -inf]`, etc...). Which is never processed, and is used to pad the batch of states only.
 
-Optionally, you can define a static `get_states_indices` method that assigns a unique integer number to each state if the environment allows it, and a `n_states` property that returns an integer representing the number of states (excluding $s_f$) in the environment. `get_terminating_states_indices` can also be implemented and serves the purpose of uniquely identifying terminating states of the environment.
+For discrete environments, the action set is represented with the set $\{0, \dots, n_{actions} - 1\}$, where the $(n_{actions})$-th action always corresponds to the exit or terminate action, i.e. that results in a transition of the type $s \rightarrow s_f$, but not all actions are possible at all states. Each `States` object is endowed with two extra attributes: `forward_masks` and `backward_masks`, representing which actions are allowed at each state and which actions could have led to each state, respectively. Such states are instances of the `DiscreteStates` abstract subclass of `States`. The `forward_masks` tensor is of shape `(*batch_shape, n_{actions})`, and `backward_masks` is of shape `(*batch_shape, n_{actions} - 1)`. Each subclass of `DiscreteStates` needs to implement the `update_masks` function, that uses the environment's logic to define the two tensors.
 
-For more details, take a look at [HyperGrid](https://github.com/saleml/gfn/blob/master/src/gfn/envs/hypergrid.py), an environment where all states are terminating states, or at [DiscreteEBM](https://github.com/saleml/gfn/blob/master/src/gfn/envs/discrete_ebm.py), where all trajectories are of the same length but only some states are terminating.
+### Actions
+Actions should be though of as internal actions of an agent building a compositional object. They correspond to transitions $s \rightarrow s'$. An abstract `Actions` class is provided. It is automatically subclassed for discrete environments, but needs to be manually subclassed otherwise.
 
-### Other containers
+Similar to `States` objects, each action is a tensor of shape `(*batch_shape, *action_shape)`. For discrete environments for instances, `action_shape = (1,)`, representing an integer between $0$ and $n_{actions} - 1$.
 
-Besides the `States` class, other containers of states are available:
+Additionally, each subclass needs to define two more class variable tensors:
+- `dummy_action`: A tensor that is padded to sequences of actions in the shorter trajectories of a batch of trajectories. It is `[-1]` for discrete environments.
+- `exit_action`: A tensor that corresponds to the termination action. It is `[n_{actions} - 1]` fo discrete environments.
 
-- [Transitions](https://github.com/saleml/gfn/blob/master/src/gfn/containers/transitions.py), representing a batch of transitions $s \rightarrow s'$.
-- [Trajectories](https://github.com/saleml/gfn/blob/master/src/gfn/containers/trajectories.py), representing a batch of complete trajectories $\tau = s_0 \rightarrow s_1 \rightarrow \dots \rightarrow s_n \rightarrow s_f$.
+### Containers
 
-These containers can either be instantiated using a `States` object, or can be initialized as empty containers that can be populated on the fly, allowing the usage of [ReplayBuffer](https://github.com/saleml/gfn/blob/master/src/gfn/containers/replay_buffer.py)s.
+Containers are collections of `States`, along with other information, such as reward values, or densities $p(s' \mid s)$. Two containers are available:
 
-They inherit from the base `Container` [class](https://github.com/saleml/gfn/blob/master/src/gfn/containers/base.py), indicating some helpful methods.
+- [Transitions](https://github.com/saleml/torchgfn/tree/master/src/gfn/containers/transitions.py), representing a batch of transitions $s \rightarrow s'$.
+- [Trajectories](https://github.com/saleml/torchgfn/tree/master/src/gfn/containers/trajectories.py), representing a batch of complete trajectories $\tau = s_0 \rightarrow s_1 \rightarrow \dots \rightarrow s_n \rightarrow s_f$.
 
-In most cases, one needs to sample complete trajectories. From a batch of trajectories, a batch of states and batch of transitions can be defined using `Trajectories.to_transitions()` and `Trajectories.to_states()`. These exclude meaningless transitions and states that were added to the batch of trajectories to allow for efficient batching.
+These containers can either be instantiated using a `States` object, or can be initialized as empty containers that can be populated on the fly, allowing the usage of the[ReplayBuffer](https://github.com/saleml/torchgfn/tree/master/src/gfn/containers/replay_buffer.py) class.
 
-### Estimators and Modules
+They inherit from the base `Container` [class](https://github.com/saleml/torchgfn/tree/master/src/gfn/containers/base.py), indicating some helpful methods.
 
-Training GFlowNets requires one or multiple estimators. As of now, only discrete environments are handled. All estimators are subclasses of [FunctionEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py), implementing a `__call__` function that takes as input a batch of [States](https://github.com/saleml/gfn/blob/master/src/gfn/containers/states.py).
+In most cases, one needs to sample complete trajectories. From a batch of trajectories, a batch of states and batch of transitions can be defined using `Trajectories.to_transitions()` and `Trajectories.to_states()`. These exclude meaningless transitions and dummy states that were added to the batch of trajectories to allow for efficient batching.
 
-- [LogEdgeFlowEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, n_actions)` tensor representing $\log F(s \rightarrow s')$, including when $s' = s_f$.
-- [LogStateFlowEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, 1)` tensor representing $\log F(s)$. When used with `forward_looking=True`, $\log F(s)$ is parametrized as the sum of a function approximator and $\log R(s)$ - which is only possible for environments where all states are terminating.
-- [LogitPFEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, n_actions)` tensor representing $logit(s' \mid s)$, such that $P_F(s' \mid s) = softmax_{s'}\ logit(s' \mid s)$, including when $s' = s_f$.
-- [LogitPBEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, n_actions - 1)` tensor representing $logit(s' \mid s)$, such that $P_B(s' \mid s) = softmax_{s'}\ logit(s' \mid s)$.
+### Modules
 
-Defining an estimator requires the environment, and a [module](https://github.com/saleml/gfn/blob/master/src/gfn/modules.py) instance. Modules inherit from the [GFNModule](https://github.com/saleml/gfn/blob/master/src/gfn/modules.py) class, which can be seen as an extension of `torch.nn.Module`. Alternatively, a module is created by providing which module type to use (e.g. "NeuralNet" or "Uniform" or "Zero"). A Basic MLP is provided as the [NeuralNet](https://github.com/saleml/gfn/blob/master/src/gfn/modules.py) class, but any function approximator should be possible.
+Training GFlowNets requires one or multiple estimators, called `GFNModule`s, which is an abstract subclass of `torch.nn.Module`. In addition to the usual `forward` function, `GFNModule`s need to implement a `required_output_dim` attribute, to ensure that the outputs have the required dimension for the task at hand; and some (but not all) need to implement a `to_probability_distribution` function. They take the environment `env` as an input at initialization.
+- `DiscretePolicyEstimator` is a `GFNModule` that defines the policies $P_F(. \mid s)$ and $P_B(. \mid s)$ for discrete environments. When `backward=False`, the required output dimension is `n = env.n_actions`, and when `backward=True`, it is `n = env.n_actions - 1`. These `n` numbers represent the logits of a Categorical distribution. Additionally, they include exploration parameters, in order to define a tempered version of $P_F$, or a mixture of $P_F$ with a uniform distribution. Naturally, before defining the Categorical distributions, forbidden actions (that are encoded in the `DiscreteStates`' masks attributes), are given 0 probability by setting the corresponding logit to $-\infty$.
+- `ScalarModule` is a simple module with required output dimension 1. It is useful to define log-state flows $\log F(s)$.
 
-Said differently, a `States` object is first transformed via the environment's preprocessor to a `(*batch_shape, *output_shape)` float tensor. The preprocessor's output shape should match the module input shape (if any). The preprocessed states are then passed as inputs to the module, returning the desired output (either flows or probabilities over children in the DAG).
+For non-discrete environments, the user needs to specify their own policies $P_F$ and $P_B$. The module, taking as input a batch of states (as a `States`) object, should return the batched parameters of a `torch.Distribution`. The distribution depends on the environment. The `to_probability_distribution` function handles the conversion of the parameter outputs to an actual batched `Distribution` object, that implements at least the `sample` and `log_prob` functions. An example is provided [here](https://github.com/saleml/torchgfn/tree/master/src/gfn/gym/helpers/box_utils.py), for a square environment in which the forward policy has support either on a quarter disk, or on an arc-circle, such that the angle, and the radius (for the quarter disk part) are scaled samples from a mixture of Beta distributions. The provided example shows an intricate scenario, and it is not expected that user defined environment need this much level of details.
 
-Each module has a `named_parameters` functions that returns a dictionary of the learnable parameters. This attribute is transferred to the corresponding estimator.
+In all `GFNModule`s, note that the input of the `forward` function is a `States` object. Meaning that they first need to be transformed to tensors. However, `states.tensor` does not necessarily include the structure that a neural network can used to generalize. It is common in these scenarios to have a function that transforms these raw tensor states to ones where the structure is clearer, via a `Preprocessor` object, that is part of the environment. More on this [here](https://github.com/saleml/torchgfn/tree/master/tutorials/ENV.md). The default preprocessor of an environment is the identity preprocessor. The `forward` pass thus first calls the `preprocessor` attribute of the environment on `States`, before performing any transformation.
 
-Additionally, a [LogZEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py) is provided, which is a container for a scalar tensor representing $\log Z$, the log-partition function, useful for the Trajectory Balance loss for example. This estimator also has a `named_parameters` function.
+For discrete environments, tabular modules are provided, where a lookup table is used instead of a neural network. Additionally, a `UniformPB` module is provided, implementing a uniform backward policy.
 
 ### Samplers
 
-An [ActionsSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/actions_samplers.py) object defines how actions are sampled at each state of the DAG. As of now, only [DiscreteActionsSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/actions_samplers.py)s are implemented. The require an estimator (of $P_F$, $P_B$, or edge flows) defining the action probabilities. These estimators can contain any type of modules (including random action sampling for example). A [BackwardDiscreteActionsSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/actions_samplers.py) class is provided to sample parents of a state, which is helpful to sample trajectories starting from their last states.
+A [Sampler](https://github.com/saleml/torchgfn/tree/master/src/gfn/samplers.py) object defines how actions are sampled (`sample_actions()`) at each state, and trajectories  (`sample_trajectories()`), which can sample a batch of trajectories starting from a given set of initial states or starting from $s_0$. It requires a `GFNModule` that implements the `to_probability_distribution` function.
 
-They are at the core of [TrajectoriesSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/trajectories_sampler.py)s, which implements the `sample_trajectories` method, that sample a batch of trajectories starting from a given set of initial states or starting from $s_0$.
 
 ### Losses
 
-GFlowNets can be trained with different losses, each of which requires a different parametrization. A parametrization is a dataclass, which can be seen as a container of different estimators. Each parametrization defines a distribution over trajectories, via the `parametrization.Pi` method, and a distribution over terminating states, via the `parametrization.P_T` method. Both distributions should be instances of the classes defined [here](https://github.com/saleml/gfn/blob/master/src/gfn/distributions.py).
-
-The base classes for losses and parametrizations are provided [here](https://github.com/saleml/gfn/blob/master/src/gfn/losses/base.py).
+GFlowNets can be trained with different losses, each of which requires a different parametrization, which we call in this library a `GFlowNet`. A `GFlowNet` is a `GFNModule` that includes one or multiple `GFNModules`, at least one of which implements a `to_probability_distribution` function. They also need to implement a `loss` function, that takes as input either states, transitions, or trajectories, depending on the loss.
 
 Currently, the implemented losses are:
 
 - Flow Matching
-- Detailed Balance
+- Detailed Balance (and it's modified variant).
 - Trajectory Balance
-- Sub-Trajectory Balance. By default, each sub-trajectory is weighted geometrically (within the trajectory) depending on its length. This corresponds to the strategy defined [here](https://www.semanticscholar.org/reader/f2c32fe3f7f3e2e9d36d833e32ec55fc93f900f5). Other strategies exist and are implemented [here](https://github.com/saleml/gfn/blob/master/src/gfn/losses/sub_trajectory_balance.py).
+- Sub-Trajectory Balance. By default, each sub-trajectory is weighted geometrically (within the trajectory) depending on its length. This corresponds to the strategy defined [here](https://www.semanticscholar.org/reader/f2c32fe3f7f3e2e9d36d833e32ec55fc93f900f5). Other strategies exist and are implemented [here](https://github.com/saleml/torchgfn/tree/master/src/gfn/losses/sub_trajectory_balance.py).
 - Log Partition Variance loss. Introduced [here](https://arxiv.org/abs/2302.05446)
 
-### Solving for the flows using Dynamic Programming
-
-A simple script that propagates trajectories rewards through the DAG to define edge flows in a deterministic way (by visiting each edge once only) is provided [here](https://github.com/saleml/gfn/blob/master/scripts/dynamic_programming.py). Do not use the script on large environments !
-
+# Scripts
+Example scripts are provided [here](https://github.com/saleml/torchgfn/tree/master/tutorials/examples/). They can be used to reproduce published results in the HyperGrid environment, and the Box environment.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

