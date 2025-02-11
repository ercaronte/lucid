<img src="https://github.com/ercaronte/lucid/raw/master/notebooks/static/channels-visualizations.jpg" width="782"></img>

# Lucid

<!--*DeepDream, but sane. Home of cats, dreams, and interpretable neural networks.*-->

[![PyPI project status](https://img.shields.io/pypi/status/Lucid.svg)]()
[![Travis build status](https://img.shields.io/travis/tensorflow/lucid.svg)](https://travis-ci.org/tensorflow/lucid)
[![Code coverage](https://img.shields.io/coveralls/github/tensorflow/lucid.svg)](https://coveralls.io/github/tensorflow/lucid)
[![Supported Python version](https://img.shields.io/pypi/pyversions/Lucid.svg)]()
[![PyPI release version](https://img.shields.io/pypi/v/Lucid.svg)](https://pypi.org/project/Lucid/)


Lucid is a collection of infrastructure and tools for research in neural
network interpretability.

This repository is a fork of the original [tensorflow repository](https://github.com/tensorflow/lucid), that has been modified to support tensorflow 2 since Colab does no longer support the `%tensorflow_version 1.x` compatibility magic command.

**Lucid is research code, not production code. We provide no guarantee it will work for your use case. Lucid is maintained by volunteers who are unable to provide significant technical support.**

* [📓 **Notebooks**](#notebooks) -- Get started without any setup!
* [📚 **Reading**](#recommended-reading) -- Learn more about visualizing neural nets.
* [💬 **Community**](#community) -- Want to get involved? Please reach out!
* [🔧 **Additional Information**](#additional-information) -- Licensing, code style, etc.
* [🔬 **Start Doing Research!**](https://github.com/tensorflow/lucid/issues?utf8=%E2%9C%93&q=is%3Aissue+label%3Aresearch) -- Want to get involved? We're trying to research openly!
* [📦 **Visualize your own model**](https://github.com/tensorflow/lucid/wiki/Importing-Models-into-Lucid) -- How to import your own model for visualization


# Notebooks

Start visualizing neural networks ***with no setup***. The following notebooks
run right from your browser, thanks to [Colaboratory](https://colab.research.google.com/notebooks/welcome.ipynb). It's a Jupyter notebook environment that requires no setup to use and runs entirely in the cloud.

You can run the notebooks on your local machine, too. Clone the repository and find them in the `notebooks` subfolder. You will need to run a local instance of the [Jupyter notebook environment](http://jupyter.org/install.html) to execute them.

## Tutorial Notebooks

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/tutorial.ipynb">
<img src="https://storage.googleapis.com/lucid-static/common/stickers/colab-tutorial.png" width="500" alt=""></img>
</a-->
- [Tutorial notebook](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/tutorial.ipynb)

  This tutorial quickly introduces Lucid, a network for visualizing neural networks. Lucid is a kind of spiritual successor to DeepDream, but provides flexible abstractions so that it can be used for a wide range of interpretability research.

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/modelzoo.ipynb">
<img src="https://storage.googleapis.com/lucid-static/common/stickers/colab-modelzoo.png" width="500" alt=""></img>
</a-->
- [Modelzoo notebook](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/modelzoo.ipynb)

  If you want to study techniques for visualizing and understanding neural networks, it's important to be able to try your experiments on multiple models. <br>
  Lucid is a library for visualizing neural networks. As of lucid v0.3, we provide a consistent API for interacting with 27 different vision models.

<!--If you want to study techniques for visualizing and understanding neural networks, it's important to be able to try your experiments on multiple models. As of lucid v0.3, we provide a consistent API for interacting with 27 different vision models.-->

## Feature Visualization Notebooks
*Notebooks corresponding to the [Feature Visualization](https://distill.pub/2017/feature-visualization/) article*

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/feature-visualization/negative_neurons.ipynb">
<img src="https://storage.googleapis.com/lucid-static/feature-visualization/stickers/colab-neuron-negative.png" width="500" alt=""></img>
</a-->
- [Negative Neurons](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/feature-visualization/negative_neurons.ipynb)

  This notebook reproduces the negative channel visualizations shown in the article.

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/feature-visualization/neuron_diversity.ipynb">
<img src="https://storage.googleapis.com/lucid-static/feature-visualization/stickers/colab-neuron-diversity.png" width="500" alt=""></img>
</a-->

- [Neuron diversity](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/feature-visualization/neuron_diversity.ipynb)

  This notebook reproduces the neuron diversity visualizations shown in the article.

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/feature-visualization/neuron_interaction.ipynb">
<img src="https://storage.googleapis.com/lucid-static/feature-visualization/stickers/colab-neuron-interaction.png" width="500" alt=""></img>
</a-->
- [Neuron interaction](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/feature-visualization/neuron_interaction.ipynb)

  This notebook reproduces some visualizations created by interacting different neurons as described in the article.

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/feature-visualization/regularization.ipynb">
<img src="https://storage.googleapis.com/lucid-static/feature-visualization/stickers/colab-regularization.png" width="500" alt=""></img>
</a-->
- [Regularization](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/feature-visualization/regularization.ipynb)

  This notebook describes the feature visualization algorithms used in the article.

## Building Blocks Notebooks
*Notebooks corresponding to the [Building Blocks of Interpretability](https://distill.pub/2018/building-blocks/) article*

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/building-blocks/SemanticDictionary.ipynb">
<img src="https://storage.googleapis.com/lucid-static/building-blocks/stickers/colab-semantic-dict.png" width="500" alt=""></img>
</a-->
- [Semantic Dictionary](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/building-blocks/SemanticDictionary.ipynb)

  This notebook studies **semantic dictionaries**. The basic idea of semantic dictionaries is to marry neuron activations to visualizations of those neurons, transforming them from abstract vectors to something more meaningful to humans. Semantic dictionaries can also be applied to other bases, such as rotated versions of activations space that try to disentangle neurons.

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/building-blocks/ActivationGrid.ipynb">
<img src="https://storage.googleapis.com/lucid-static/building-blocks/stickers/colab-grid.png" width="500" alt=""></img>
</a-->
- [Activation Grid](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/building-blocks/ActivationGrid.ipynb)

  This notebook studies **activation grids** a technique for visualizing how a network "understood" an image at a particular layer.

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/building-blocks/AttrSpatial.ipynb">
<img src="https://storage.googleapis.com/lucid-static/building-blocks/stickers/colab-spatial-attr.png" width="500" alt=""></img>
</a-->
- [Spacial Attribution](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/building-blocks/AttrSpatial.ipynb)

  This notebook demonstrates **Spatial Attribution**, a technique for exploring how detectors a different spatial positions in the network effected its output.

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/building-blocks/AttrChannel.ipynb">
<img src="https://storage.googleapis.com/lucid-static/building-blocks/stickers/colab-channel-attr.png" width="500" alt=""></img>
</a-->
- [Channel Attribution](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/building-blocks/AttrChannel.ipynb)

  This notebook demonstrates **Channel Attribution**, a technique for exploring how different detectors in the network effected its output.

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/building-blocks/NeuronGroups.ipynb">
<img src="https://storage.googleapis.com/lucid-static/building-blocks/stickers/colab-neuron-groups.png" width="500" alt=""></img>
</a-->
- [Neuron Groups](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/building-blocks/NeuronGroups.ipynb)

  This notebook demonstrates **Neuron Groups**, a technique for exploring how detectors a different spatial positions in the network effected its output. ...

## Differentiable Image Parameterizations Notebooks
*Notebooks corresponding to the [Differentiable Image Parameterizations](https://distill.pub/2018/differentiable-parameterizations/) article*

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/differentiable-parameterizations/aligned_interpolation.ipynb">
<img src="https://storage.googleapis.com/lucid-static/differentiable-parameterizations/stickers/colab-interpolate.png" width="500" alt=""></img>
</a-->
- [Aligned interpolation](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/differentiable-parameterizations/aligned_interpolation.ipynb)

  This notebook uses the Lucid library to create a visualizations that interpolates between two feature visualizations.

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/differentiable-parameterizations/style_transfer_2d.ipynb">
<img src="https://storage.googleapis.com/lucid-static/differentiable-parameterizations/stickers/colab-style-beyond-vgg.png" width="500" alt=""></img>
</a-->
- [2D Style transfer](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/differentiable-parameterizations/style_transfer_2d.ipynb)

  This notebook uses Lucid to perform style transfer between two images, and show how different parameterizations affect that process.

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/differentiable-parameterizations/xy2rgb.ipynb">
<img src="https://storage.googleapis.com/lucid-static/differentiable-parameterizations/stickers/colab-xy2rgb.png" width="500" alt=""></img>
</a-->
- [Compositional Pattern Producing Network](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/differentiable-parameterizations/xy2rgb.ipynb)

  This notebook uses Lucid to produce aesthetically pleasing feature visualizations using a [Differentiable Image Parameterization](https://distill.pub/2018/differentiable-parameterizations/#section-xy2rgb) called a **Compositional Pattern Producing Network** (CPPN).

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/differentiable-parameterizations/transparency.ipynb">
<img src="https://storage.googleapis.com/lucid-static/differentiable-parameterizations/stickers/colab-transparent.png" width="500" alt=""></img>
</a-->
- [Generating semi-transparent Feature Visualizations](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/differentiable-parameterizations/transparency.ipynb)

  This notebook uses Lucid to produce semi-transparent feature visualizations using a [Differentiable Image Parameterization](https://distill.pub/2018/differentiable-parameterizations/#section-xy2rgb) with an extra **alpha channel**.

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/differentiable-parameterizations/texture_synth_3d.ipynb">
<img src="https://storage.googleapis.com/lucid-static/differentiable-parameterizations/stickers/colab-3d-texture.png" width="500" alt=""></img>
</a-->
- [3D Feature Visualization](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/differentiable-parameterizations/texture_synth_3d.ipynb)

  This notebook uses Lucid to produce feature visualizations on 3D mesh surfaces by using a [Differentiable Image Parameterization](https://distill.pub/2018/differentiable-parameterizations/#section-featureviz-3d).

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/differentiable-parameterizations/style_transfer_3d.ipynb">
<img src="https://storage.googleapis.com/lucid-static/differentiable-parameterizations/stickers/colab-3d-style.png" width="500" alt=""></img>
</a-->
- [3D Style Transfer](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/differentiable-parameterizations/style_transfer_3d.ipynb)

  This notebook uses Lucid to implement style transfer from a textured 3D model and a style image onto a new texture for the 3D model by using a [Differentiable Image Parameterization](https://distill.pub/2018/differentiable-parameterizations/#section-style-transfer-3d).


## Activation Atlas Notebooks
*Notebooks corresponding to the [Activation Atlas](https://distill.pub/2019/activation-atlas/) article*

<a href="https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/activation-atlas/activation-atlas-collect.ipynb">
<img src="https://storage.googleapis.com/modelzoo/tmp/activation-atlas/stickers/lucid-notebook-1-collect.png" width="500" alt="Collecting activations"/>
</a>

<a href="https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/activation-atlas/activation-atlas-simple.ipynb">
<img src="https://storage.googleapis.com/modelzoo/tmp/activation-atlas/stickers/lucid-notebook-2-atlas.png" width="500" alt="Simple activation atlas"/>
</a>

<a href="https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/activation-atlas/class-activation-atlas.ipynb">
<img src="https://storage.googleapis.com/modelzoo/tmp/activation-atlas/stickers/lucid-notebook-3-class-atlas.png" width="500" alt="Class activation atlas"/>
</a>

<a href="https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/activation-atlas/activation-atlas-adversarial.ipynb">
<img src="https://storage.googleapis.com/modelzoo/tmp/activation-atlas/stickers/lucid-notebook-4-patches.png" width="500" alt="Activation atlas patches"/>
</a>

## Miscellaneous Notebooks

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/misc/feature_inversion_caricatures.ipynb">
<img src="https://storage.googleapis.com/lucid-static/misc/stickers/colab-feature-inversion.ipynb.png" width="500" alt=""/>
</a-->
- [Feature Inversion Caricatures](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/misc/feature_inversion_caricatures.ipynb)

  This notebook uses Lucid to produce feature inversion caricatures that are similar in spirit to the activation grids in [The Building Blocks of Interpretability](https://distill.pub/2018/building-blocks/).

<!--a href="https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/misc/neuron_interaction_grids.ipynb">
<img src="https://storage.googleapis.com/lucid-static/misc/stickers/colab-interaction-grid.png" width="500" alt=""/>
</a-->
- [Neuron Interaction Grids](https://colab.research.google.com/github/ercaronte/lucid/blob/master/notebooks/misc/neuron_interaction_grids.ipynb)

  This notebook uses Lucid to produce grids showing how neurons different neurons interact.

# Recommended Reading

* [Feature Visualization](https://distill.pub/2017/feature-visualization/)
* [The Building Blocks of Interpretability](https://distill.pub/2018/building-blocks/)
* [Using Artiﬁcial Intelligence to Augment Human Intelligence](https://distill.pub/2017/aia/)
* [Visualizing Representations: Deep Learning and Human Beings](http://colah.github.io/posts/2015-01-Visualizing-Representations/)
* [Differentiable Image Parameterizations](https://distill.pub/2018/differentiable-parameterizations/)
* [Activation Atlas](https://distill.pub/2019/activation-atlas/)

## Related Talks
* [Lessons from a year of Distill ML Research](https://www.youtube.com/watch?v=jlZsgUZaIyY) (Shan Carter, OpenVisConf)
* [Machine Learning for Visualization](https://www.youtube.com/watch?v=6n-kCYn0zxU) (Ian Johnson, OpenVisConf)

# Community

We're in `#proj-lucid` on the Distill slack ([join link](http://slack.distill.pub)).

We'd love to see more people doing research in this space!

<br>

# Additional Information

## License and Disclaimer

You may use this software under the Apache 2.0 License. See [LICENSE](LICENSE).

This project is research code. It is not an official Google product.

## Special consideration for TensorFlow dependency

Lucid requires `tensorflow`, but does not explicitly depend on it in `setup.py`. Due to the way [tensorflow is packaged](https://github.com/tensorflow/tensorflow/issues/7166) and some deficiencies in how pip handles dependencies, specifying either the GPU or the non-GPU version of tensorflow will conflict with the version of tensorflow your already may have installed.

If you don't want to add your own dependency on tensorflow, you can specify which tensorflow version you want lucid to install by selecting from `extras_require` like so: `lucid[tf]` or `lucid[tf_gpu]`.

**In actual practice, we recommend you use your already installed version of tensorflow.**
