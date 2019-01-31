# Colab IClojure

This Repo has some templates that will allow you to run Clojure code on [Google Colaboratory](https://colab.research.google.com/notebooks/welcome.ipynb)
![](https://c1.staticflickr.com/8/7858/46881073892_8f6fa874c7_b.jpg)
It uses [IClojure](https://github.com/HCADatalab/IClojure) as the Jupyter kernel

## Instructions

This is a two step process, there is no automated way to do this so far. The first step is to install the Clojure kernel. The next step is to upload a notebook and connect to the kernel runtime.

## Install the Clojure Kernel

- Go to the Colaboratory and hit *File/upload-notebook*  - Either copy the `install_iclojure.ipynb` directly or use this [github link](https://github.com/gigasquid/colab-iclojure/blob/master/install_iclojure.ipynb)
- Execute all the cells, one by one - the last cell should show that you now have the iclojure kenel

```
Available kernels:
  iclojure    /root/.local/share/jupyter/kernels/iclojure
  python2     /usr/local/share/jupyter/kernels/python2
  python3     /usr/local/share/jupyter/kernels/python3
  swift       /usr/local/share/jupyter/kernels/swift
```

## Upload an IClojure notebook and connect

- Hit *File/upload-notebooke*. Next upload the `iclojure_with_deps_example.ipynb`. Make sure you do not `reset your runtime`.
- Execute the first cell `(+ 1 1)`. It should connect to the IClojure kernel and execute.
- You can add depenencies with `/cp`
- Hack and glory await!

## MXNet examples
If you want to do an MXNet example, you can use a similar process above using these two notebooks:
* mxnet/clojure_with_mxnet_example.ipynb
* mxnet/install_iclojure_with_mxnet.ipynb
