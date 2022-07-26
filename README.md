# gsoc2022-Bhavesh_Misra

#Issue_1763

The changes have been made in the Evaluator.py, and the following changes are to be made in the DOckerfile and Dockerfile.base to see the changes.

Changes in the Dockerfile:-
At the 2nd last line of the DOckerfile, add this line 

"COPY human_detection/ /RoboticsAcademy/exercises/human_detection/"

Changes in the Dockerfile.base:-

Python 3 dependencies installed by pip (line 140)
RUN python3 -m pip install argparse argcomplete coverage cerberus empy jinja2 kconfiglib \
		matplotlib==3.0.* numpy nunavut==1.1.0 packaging pkgconfig pyros-genmsg pyulog \
		pyyaml requests serial six toml psutil pyulog wheel onnxruntime Pillow opencv-python netron seaborn
    
Basically add seaborn in the DOckerfile.base to create an image, with Seaborn installed , so as to see the updated plots.   

Steps:-
1) Follow these changes
2) Create a new docker image, run the exercise by creating a docker container, and copy the contents (basically the whole human_detection exercise) in the docker container
3) You should be able to see the new benchmarking graph pop up
