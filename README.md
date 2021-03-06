# spn-poon-2011
Modification of original implementation of code from 
Poon,Domingos, **Sum-Product Network: a New Deep Architecture**, UAI 2011
at [http://spn.cs.washington.edu/spn/](http://spn.cs.washington.edu/spn/), for SPN MNIST missing data experiments.

1. Generate MNIST data for training by running `python data/generate_mnist.py` (path to raw MNIST data assumes that [https://github.com/HUJI-Deep/Generative-ConvACs/blob/master/exp/mnist/generate_mnist.py](https://github.com/HUJI-Deep/Generative-ConvACs/blob/master/exp/mnist/generate_mnist.py) has already been run).
2. Follow setup instructions from original code, then compile from `code` folder using `javac -cp .:$MPJ_HOME/lib/mpj.jar -d bin @source.txt`
3. From the `bin` folder, run `mpjrun.sh -np <NUM_PROCS> eval.Run -d M -nsg 1 -ns <NUM_PROCS-1> > ../../results/mnist_run.log` where `NUM_PROCS` is the number of processors available.
