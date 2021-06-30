# Finding_Lanes

In this project, Python and OpenCV were used to find lane lines in the road images.  

The following techniques are used:

- Color Selection
- Canny Edge Detection
- Region of Interest Selection
- Hough Transform Line Detection

Finally, I applied all the techniques to process video clips to find lane lines in them.

## How to Reproduce the results

To set up the conda environment, execute the following:

```python
conda env create -f environment.yaml
```

Then, activate the environment:

```python
conda activate car-finding-lane-lines
```

Start the jupyter notebook:

```bash
python Finding_Lane.py
```
---

The following explains what the codes in the notebook do.

### Test Video link 
you can download the video in this [Link](https://drive.google.com/file/d/1WiebkAXB2UIpNpgOJSavrdBHL7m98he1/view?usp=sharing).

