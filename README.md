# Lucid
*DeepDream, but sane. Home of cats, dreams, and interpretable neural networks.*

Lucid is a collection of infrastructure and tools for research in neural network interpretability. 

In particular, it provides state of the art implementations of [feature visualization techniques](https://distill.pub/2017/feature-visualization/), and flexible abstractions that make it very easy to explore new research directions.

Quick start: [lucid tutorial]() (TODO) -- runs in your web browser, get started visualizing neural networks in <5 min.


# Project Structure

How lucid is structured:

* [**modelzoo**]():
  Easily import models for visualization
* [**optvis**]():
  Framework for optimization-based [feature visualization](https://distill.pub/2017/feature-visualization/)
* [**scratch**]():
  Incubating code that needs to be shared between notebooks.
* [**misc**]():
  More mature code that doesn't fit into a large cluster.
* [**recipes**]():
  Less general code that makes a particular visualization.

Note that we do a lot of our research in colab notebooks and transition code here as it matures.


# License and Disclaimer

You may use this software under the Apache 2.0 License. See [LICENSE](LICENSE).

This project is research code. It is not an official Google product. 