# Introduction to Cellpose

[**Cellpose**](https://www.cellpose.org) is a **free**, **open-source** software tool for **automatic cell segmentation** using **deep learning**. It is designed for **biological image analysis**, working on a wide range of microscopy images without requiring parameter tuning or extensive training data. It is a generalist image segmentation tool.

At its core, **Cellpose** uses a **pretrained deep neural network** to segment cells based on learned features. It supports both **2D** and **3D datasets**, and can handle a variety of **morphologies**, including nuclei, cytoplasm, whole cells, and irregular structures. Users can also **train custom models** using their own data if the pretrained model doesn't fit their needs.

<div align="center">
    <img src="https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41592-020-01018-x/MediaObjects/41592_2020_1018_Fig1_HTML.png?as=webp" alt="Cellpose Flow Fields" width="600">
</div>

<br>

The project is well-supported with **documentation, tutorials, and example datasets**, all available on the [official website](https://www.cellpose.org) and [GitHub repository](https://github.com/MouseLand/cellpose).

## Download and Install Cellpose

**Cellpose** is available via:

* A **Python package** (recommended for scripting and integration into pipelines)
* A **Graphical User Interface (GUI)** for interactive use

<div align="center">
    <img src="../../../_static/images/cellpose/starting_window.png" alt="Cellpose GUI" width="600">
</div>

Below are the instructions to install Cellpose using [`uv`](https://docs.astral.sh/uv/).

You can use `uv` to install Cellpose in two ways:

1. **Direct execution**: Use `uv` to automatically handle environment creation and run the GUI directly
2. **Manual environment setup**: Create a virtual environment first, then install Cellpose within that environment

### 1. Direct Execution with uv

By simply running the command below, `uv` will create a virtual environment, install Cellpose, and launch the GUI (it might take a little while the first time you run this command but after that it will be very quick).

```bash
uvx --from "cellpose[gui]" cellpose
```

### 2. Manual Environment Setup

If you need to use Cellpose for scripting and integration into pipelines, it is then useful to set up a virtual environment manually. Here are the steps:

**1. Create a new virtual environment:**

```bash
python -m venv cellpose-env
```

**2. Activate the virtual environment:**

```bash
# On Linux or macOS
source cellpose-env/bin/activate
# On Windows use 
cellpose-env\Scripts\activate
```

**3. Install Cellpose:**

```bash
uv pip install cellpose
```

If you will also need to run the Cellpose through the GUI, you should install it with GUI support:

```bash
uv pip install "cellpose[gui]"
```

And then, to launch the GUI:

```bash
python -m cellpose # (or simply cellpose)
```

## What's Next?

In the next sections, we will briefly demonstrate [how to use Cellpose through the GUI](cellpose_gui.md) and then focus more on how to use it in scripts and pipelines to automate the segmentation process on multiple images. We will also show how to train custom models if the pretrained model does not fit your specific needs.
