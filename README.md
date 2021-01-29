## WikiGaze

We propose WikiGaze, a state-of-the-art approach to utilize readers' participation in Wikipedia analysis. We capture readers' conceptual reception of an article in the form of their eye gaze pattern over the article. Applying eye-tracking to reading pattern analysis requires a fundamental trade-off between the invasiveness of the eye tracker and the accuracy of the estimated gaze points. Instead of using an expensive, invasive device like Tobii; we propose to use lightweight desk-mounted/laptop camera to perform eye gaze tracking with the help of some computer vision technique.

* Repositiory: Anonymized temporary Github Repo [https://github.com/WikiGaze/Wikipedia-readers-gaze] 
* License: 3-Clause BSD
# Supplementary Material

Google Scholar Experiment details: [Google_scholar.pdf]
Leaderboard Creation Algorithms: [Leaderboard_algos.pdf]

# Video Explaination

<iframe width="560" height="315" src="https://youtube.com/embed/AtimebDAfJ0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Installation for Mac OS X / Ubuntu / Windows systems

### Scripted Installation
* Install Opengazer: [https://github.com/qiffp/OpenGazer] for Mac OS X or Ubuntu systems
* Install Netgazer: [https://sourceforge.net/projects/netgazer/] for Windows systems
* Open a terminal and run:
```bash
cd opengazer
sudo bash dependencies.sh
make
```

### Manual Installation 
python3-pip

* PyQt5
* MSS
* pynput
* OpenCv
* Numpy
* pytesseract
* Wnck
* Gtk
* Tensorflow

### apt-get

* tesseract-ocr

### Installing OCR tool

```bash
sudo apt-get install tesseract-ocr
```
## Config Files

* main_cofig
    1. [0] Determines when to start or stop capture_gaze script.
    1. [1] Determines when to store the captured gaze values into a variable.
    1. [2] Determines whether the program has been successfully calibrated or not.

* config
    1. [0] Determines when to start or stop the elg_demo script to calibrate the program.
    1. [1] Determines when to open the calibration window and run the subsequent script.
    1. [2] Determines when to run the Wait GUI and script.
    1. [3] Determines when to save the captured gaze values into a file.
    1. [4] Determines when to capture the gaze values and store it into a variable.

> The number within third bracket determines the index value of that line in the file.

# Application Run

```bash
cd Integration

python new_main.py
```

# Application Usage Procedure
Participants are required to follow the following steps during dataset collection:

<ol style="list-style-type:lower-roman">
  <li>Put the camera centrally under you monitor, so that the height of your face in the image is about half of the height of the image, and close to the centre of the image. Make sure the background light level is reasonably constant across the image.</li>
  <li>Start the application and click on the summarize button.</li>
  <li>The next default step is calibration. Remember, in order for this gaze tracker to work, you must keep your head absolutely still. Press "Calibrate". You will now be asked to look at various points on the screen, indicated by a target sign. Remember: do not move your head, only your eyes!</li>
  <li>When calibration is finished, you will be redirected to your default browser automatically. There you can start reading any Wikipedia article of your choice.</li>
  <li>Upon finishing the reading session, we will display the text that you focused while reading. Do the following as per your wish:</li>
    <ol style="list-style-type:lower-roman">
    <li>If you are satisfied with the text extraction, click on the Save button.</li>
    <li>If you don’t like the text extraction, click on the discard button.</li>
    </ol>
  <li>In the end, please rate the text extraction as per your satisfaction level.</li>  
</ol>

# Survey Information
We showcase the effectiveness of the proposed editor ranking algorithm on editors’ contributions. In this evaluation, we also compare the editors’ performance under the influence of Wikipedia’s traditional leaderboard and the proposed leaderboard. Due to the lack of any similar editor ranking tool, we are unable
to provide comparative performance testing.
To evaluate the effectiveness of the proposed editor ranking approach on the contribution of editors, we conduct an experiment with the help of Introduction to Computing course students. We deploy a Wikipedia instance on our University intranet and create two new Wikipedia pages titled, “Divide and Conquer" and “Dynamic Programming". The selected topics are the categories of programming algorithms, and they are taught in the mentioned course.

We run this experiment for the duration of the last six weeks of the course. We provide students with details of both Wikipedia pages, and we ask them to make entries in both the Wikipedia pages. Students were not allowed to create new Wikipedia pages. All the edits have to be done in the above mentioned two pages only. We inform them that their weekly ranking in each leaderboard will be noted (every Sunday at 7 p.m.), and it will be considered during the final grading of
the course. We collect student's responses in the following [survey form](https://drive.google.com/file/d/1GXxvSfc02GvL4I7EkmqSjUMxDHaki_kn/view?usp=sharing). We took the consent of each participant before performing the experiment. Please find the consent [here](https://drive.google.com/file/d/1cAF9Uqr43lynVuvJMteodbJdDOo3Tri0/view?usp=sharing)
