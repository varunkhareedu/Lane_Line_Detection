# Lane Lines Detection 

Computer Vision algorithm to detect straight lane lines markings on road using OpenCV Image Processing, Color Masks, Canny Edge Detection and Hough Transform. 

![GIF](test_images_output/LaneLines.gif)

One of the most fundamental tasks in computer vision for autonomous driving is lane lines detection on road. Lane lines are painted for humans to see and follow while driving. In a very similar way, an autonomous vehicle that uses human designed infrastructure, needs to *see* the lane markings to steer accordingly and follow the road trajectory.

In this project I implemented a computer vision algorithm that processes real data recorded with the front facing camera of a vehicle driving on a California highway.
The result is a processed video that highlights the lane lines on the paved road. 

With the positions of the lane lines identified, the vehicle's offset from the lane's center can be calculated and feed a PD controller to compute the necessary steering angle. While only the lane lines detection is the scope of this project, my steering algorithm is implemented [here](https://github.com/OanaGaskey/PID-Controller)  
 
This project is implemented in Python and uses OpenCV image processing library. The source code can be found in the `finding_lane_lines.ipynb` Jupyter Notebook file above. 
