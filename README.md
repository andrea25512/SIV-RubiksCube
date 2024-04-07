# Rubik's cube faces recognition
Automatic color detection of the faces of 3x3 rubik's cubes.

The project is implemented using Jupyter Notebooks (`ipynb`), so a recent installation of Python is required.

<style>
table {
    border-collapse: collapse;
}
table, th, td {
   border: none;
}
blockquote {
    border-left: none;
    padding-left: 10px;
}
</style>

There are two versions of this project:
- `classic_cube.ipynb` works with standard rubik's cubes, e.g.:
<table>
<thead>
  <tr>
    <td><img src="Classification/real_cube3.jpg" width="200" /></td>
    <td>→</td>
    <td><img src="Classification/Output/real_cube3_id.png" width="200" /></td>
    <td>→</td>
    <td><img src="Classification/Output/real_cube3_out.png" width="600" /></td>
  </tr>
</thead>
</table>  

- `borderless.ipynb` works with stickerless cubes, e.g.:
<table>
<thead>
  <tr>
    <td><img src="Classification2/border1.jpeg" width="200"/></td>
    <td>→</td>
    <td><img src="Classification2/Output/border1_id.png" width="200" /></td>
    <td>→</td>
    <td><img src="Classification2/Output/border1_out.png" width="600" /></td>
  </tr>
</thead>
</table>


## Setting up the virtual environment

VSCode is assumed to be the code editor of choice.

### On Windows

Create a python virtual environment:
```bash
python -m venv rubiks_cube_venv
```

Activate the virtual environment:
```bash
source rubiks_cube_venv/Scripts/activate
```

Install the required python modules:
```bash
pip install -r requirements.txt
```


### On Linux
Install venv package for python:
```bash
sudo apt install python3-venv -y
```

Create a python virtual environment:
```bash
python3 -m venv rubiks_cube_venv
```

Activate the virtual environment:
```bash
source rubiks_cube_venv/bin/activate
```

Install the required python modules:
```bash
pip install -r requirements.txt
```

## Running the notebook

To execute the notebook:
- open it in VSCode
- select the kernel you just created (see [here](https://code.visualstudio.com/docs/datascience/jupyter-notebooks#_create-or-open-a-jupyter-notebook) how to do it)
- set the variable `path_to_image` to the path of the image you want to analyze
- run all the cells (see [here](https://code.visualstudio.com/docs/datascience/jupyter-notebooks#_running-cells) how to do it)

## Documentation

For the `classic_cube.ipynb` version:
- A step-by-step presentation of the inner workings (see PowerPoint [here](classic_cube_presentation.pdf))
- In depth documentation and references (see PDF [here](classic_cube_documentation.pdf))

For the `borderless.ipynb` version:
- In depth documentation and references (see PDF [here]([borderless_documentation.pdf)))
