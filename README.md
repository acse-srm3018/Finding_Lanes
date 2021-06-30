# Finding_Lanes

In this project, Python and OpenCV were used to find lane lines in the road images.  

The following techniques are used:

- Color Selection
- Canny Edge Detection
- Region of Interest Selection
- Hough Transform Line Detection

Then a pipeline consisted of 3 parts used to finding lanes:
<br>
Part One
<br>
First, I converted the images to grayscale, then I applied blur to avoid noise in the edges detection process. With the processed image I used Canny detection to find edges, this returned many irrelevant edges, so I defined vertices to make a region of interest. After that, I used Hough transformation to get lines from these edges. Finaly I drawed this lines in the original image.
<br>
Part Two
<br>
In the second part, I changed draw_lines testing each row to see if the slope was positive or negative, then I've created 2 groups of lines basead in yours slopes. Then, I calculated start and ends points to make lines with a standar lenght. Finally, I used numpy to get mean and make the function return only 2 lines with opposites slopes.
<br>
Part Three
<br>
In final part, I tested and tuned the parameters looking for the best fit in images and videos, the results were very satisfatory, but I couldn't performed well with the challenge video, I belive that more advanced and complex algorithims are needed to find lanes in that conditions.

## How to Reproduce the results

To set up the conda environment, execute the following:

```python
conda env create -f environment.yaml
```

Then, activate the environment:

```python
conda activate car-finding-lane-lines
```

Run python code in terminal:

```bash
python Finding_Lane.py
```
---

The following explains what the codes in the notebook do.

### Test Video link 
you can download the video in this [Link](https://drive.google.com/file/d/1WiebkAXB2UIpNpgOJSavrdBHL7m98he1/view?usp=sharing).

