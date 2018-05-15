# MusicGenerator

## Overview

This is the code slightly modified from [this](https://github.com/llSourcell/How_to_generate_music_in_tensorflow_LIVE). Major changes involve update code to reflect latest Tensorflow api (1.8)

## Dependencies

The program requires the following dependencies (easy to install using pip):
 * Python 3
 * tensorflow==1.8.0
 * CUDA (for using gpu, see TensorFlow [installation page](https://www.tensorflow.org/versions/master/get_started/os_setup.html#optional-install-cuda-gpus-on-linux) for more details)
 * Numpy (should be installed with TensorFlow)
 * Mido (midi library)
 * Tqdm (for the nice progression bars)
 * OpenCv (Sorry, there is no simple way to install it with python 3. It's primarily used as visualisation tool to print the piano roll so is quite optional. All OpenCv calls are contained inside the imgconnector file so if you want to use test the program without OpenCv, you can try removing the functions inside the file)

## Usage

To train the model, simply run `main.py`. Once trained, you can generate the results with `main.py --test --sample_length 500`. For more help and options, use `python main.py -h`.

To visualize the computational graph and the cost with TensorBoard, run `tensorboard --logdir save/`.


## Credits

Credits for the code go to [Conchylicultor](https://github.com/Conchylicultor/MusicGenerator). 
