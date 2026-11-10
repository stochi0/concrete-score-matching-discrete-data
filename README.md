# Concrete Score Matching

A PyTorch study implementation of
[Concrete Score Matching: Generalized Score Matching for Discrete Data](https://arxiv.org/abs/2211.00802)
by Chenlin Meng, Kristy Choi, Jiaming Song, and Stefano Ermon.

## Run

With Python 3.8+ and [uv](https://docs.astral.sh/uv/):

```sh
git clone https://github.com/stochi0/concrete-score-matching-discrete-data.git
cd concrete-score-matching-discrete-data
uv venv
uv pip install torch numpy matplotlib scikit-learn torchvision
uv run --no-project python main.py
```

[main.py](main.py) contains the model, synthetic data generation, training loss,
and Metropolis–Hastings sampler. Edit its `Config` dataclass to change the number
of states, cycle/grid neighborhood, learning rate, epochs, or sampling steps.
Training prints losses and writes `figures/1d_distributions.png` and
`figures/2d_distributions.png`. This is an implementation exercise, not a reported
reproduction of the paper's benchmarks.

## Original paper

```bibtex
@article{meng2022concrete,
  title={Concrete Score Matching: Generalized Score Matching for Discrete Data},
  author={Meng, Chenlin and Choi, Kristy and Song, Jiaming and Ermon, Stefano},
  journal={arXiv preprint arXiv:2211.00802},
  year={2022}
}
```

License: MIT.

## Citation of this implementation

<!-- BEGIN generated citations -->

```bibtex
@software{bodadeprojectconcretescorematchingdiscretedata,
  author = {Bodade, Ayush},
  title = {{Concrete Score Matching}},
  url = {https://github.com/stochi0/concrete-score-matching-discrete-data},
  note = {Software implementation; cite the original research separately. Specify the commit or version used.}
}
```

<!-- END generated citations -->
