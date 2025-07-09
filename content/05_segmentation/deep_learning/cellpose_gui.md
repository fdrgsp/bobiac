# Cellpose GUI

[**Cellpose**](https://www.cellpose.org) is a **free**, **open-source** software tool for **automatic cell segmentation** using **deep learning**. It is designed for **biological image analysis**, working on a wide range of microscopy images without requiring parameter tuning or extensive training data. It is a generalist image segmentation tool.

<div align="center">
    <img src="../../../_static/images/cellpose/starting_window.png" alt="Cellpose GUI" width="700">
</div>

At its core, **Cellpose** uses a **pretrained deep neural network** to segment cells based on learned features. It supports both **2D** and **3D datasets**, and can handle a variety of **morphologies**, including nuclei, cytoplasm, whole cells, and irregular structures. Users can also **train custom models** using their own data if the pretrained model doesn't fit their needs.

<div align="center">
    <img src="https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41592-020-01018-x/MediaObjects/41592_2020_1018_Fig1_HTML.png?as=webp" alt="Cellpose Flow Fields" width="700">
</div>

<br>

The project is well-supported with **documentation, tutorials, and example datasets**, all available on the [official website](https://www.cellpose.org) and [GitHub repository](https://github.com/MouseLand/cellpose).

## Download and Install Cellpose

**Cellpose** is available via:

* A **Python package** (recommended for scripting and integration into pipelines)
* A **Graphical User Interface (GUI)** for interactive use

To install Cellpose via Python:

```bash
pip install cellpose
```

To install the GUI:

```bash
pip install cellpose[gui]
```

For detailed installation instructions, including GPU acceleration and dependencies, see the [installation guide](https://www.cellpose.org/installation.html).

You can launch the GUI with:

```bash
python -m cellpose
```

We can also use `uv` to install and run the latest version of Cellpose using the following command:

```bash
uvx --from "cellpose[gui]" cellpose
```

## What's Next?

In the next sections, we will demonstrate:

**TODO: FEDERICO, CELLPOSE GUI DEMO AND ETC.**
