# Reference PyTorch GraphSAGE Implementation
### Author: William L. Hamilton


Basic reference PyTorch implementation of [GraphSAGE](https://github.com/williamleif/GraphSAGE).
This reference implementation is not as fast as the TensorFlow version for large graphs, but the code is easier to read and it performs better (in terms of speed) on small-graph benchmarks.
The code is also intended to be simpler, more extensible, and easier to work with than the TensorFlow version.

Currently, only supervised versions of GraphSAGE-mean and GraphSAGE-GCN are implemented. 

#### Requirements

pytorch >0.2 is required.

#### Running examples

Execute `python -m graphsage.model` to run the Cora example.
It assumes that CUDA is not being used, but modifying the run functions in `model.py` in the obvious way can change this.
There is also a pubmed example (called via the `run_pubmed` function in model.py).

### My Note

Now I updated the code so that it fits the latest pytorch.

But note that it requires Python2.7, and the same environment as specified in GraphSAGE official code.

`python -m XXX` actually loads `XXX` as a module, thus, we can do the same thing by `python mygraphsage/model.py`.

And in fact I updated it to what is runnable on Python3.7, under mygraphsage.

And it is also doable to run `model.py` after `cd mygraphsage`.