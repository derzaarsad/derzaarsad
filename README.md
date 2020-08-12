### Hi there👋!

I am currently working as a Development Engineer at an Airbus company InFactory Solutions GmbH, in Munich, Germany. Besides my paid jobs, I am also doing programming in my free time,
which you can find the repositories on my Github.

I always aim to have a potential business case for my private projects; therefore, most of my public repositories are originated from my online course activities. Nevertheless, you can see my contribution frequencies on all projects right at the bottom of this page.

In a chronological order, the followings are my project history:

### Build Automation for Gearbox Softwares

This is my very first professional project in software development. I developed a standalone application that enables
gearbox developers to do compilation and simulation tests using different software configurations before committing
their changes into the server. This application eliminated the queue time for tests almost entirely and increased
software development productivity by about 90%.

I used .NET C# Windows Forms to develop the user interface and IronPython to integrate already existing python scripts
used to parse the simulation results. In this project, I used PTC Integrity (MKS at that time) for software lifecycle
management and IBM DOORS for requirement management.

### Plane Segmentation for a 3D Reconstruction System ([KinKon](https://www.imi.kit.edu/46_2540.php))

This thesis became my first encounter with computer vision subjects as well as professional development in C++. The
project is a part of a 3D reconstruction system that used Kinect depth images as an input. I designed a module to
segment planes from a point cloud in real-time. Belong to the segmented planes are, for example, walls, floors, or
ceilings. The following is a result example of my thesis:

![plane](https://github.com/derzaarsad/derzaarsad/blob/master/imgs/plane_segmentation.png)

While doing a live 3D reconstruction, the plane segmentation algorithm was executed in every single frame. All detected
planes that belonged to the same object were merged into a single representation. To see a live 3D reconstruction
without any plane segmentation, click the image below:

[![](http://img.youtube.com/vi/v_1AAEMB2eg/0.jpg)](http://www.youtube.com/watch?v=v_1AAEMB2eg "")

### Benchmark for Online Calibration

Starting my full-time professional work, I worked on online calibration, which determines the orientation of a video
camera mounted on a vehicle relative to the vehicle coordinate system. My task was to design a benchmark to measure the
accuracy of the online calibration. Knowing the properties of coordinate system transformation, I came up with an idea
to draw a basic shape in the real world in such a way that it neglects the influence of translation and capture it as an
image using the calibrated camera. The image is then used as ground truth to compare with a virtual shape that I
projected into the image coordinate system. I used an edge detection algorithm to detect the reference shape in the
ground truth image to ensure that the measurement accuracy depends only on the camera resolution.

The following is the visualization of the SLAM technology used by the online calibration:

![sfm](https://www.all-electronics.de/wp-content/uploads/2017/05/Bild-3-Kameraposition-1024x768.png)

### Sensor Fusion-based Multi-Sensor Calibration

Multi-Sensor Calibration combined the input of multiple sensors such as camera and LIDAR with vehicle odometry to
determine not only the orientation but also the translation of the sensors relative to the vehicle coordinate system.
I implemented a strategy to filter unique data to avoid overfitting the optimization algorithm used by this application.
I also worked on the data synchronization and buffering mechanism in the software pipeline using C++ which significantly
improved the accuracy of the calibration. Lastly, as I realized that not all vehicle odometry gave 3D axis information,
so I designed a concept that enables the algorithm to replace the relative reference to another sensor than the car.

One of this application was for ESG Takamos:

[![](http://img.youtube.com/vi/XrmnZIWq46I/0.jpg)](https://www.youtube.com/watch?v=XrmnZIWq46I "")

### Head-Up-Display Test Automation with UR10 Robot

This was one of the projects that gave me chills when I saw the result.
I developed an automated system to check the optical quality of a head-up-display. When I joined the project, the robot
could not orient itself in the room, which leads to an inaccurate measurement of the head-up-display. Later on, I
effectively identified the source of the problem by testing the system using synthetic data that I generated. In the
end, I implemented a module that enables a UR10 Robot to position the camera with a very high absolute accuracy that it
can point the optical axis of the camera into any arbitrary position in the calibration plate.

### Autonomous Vehicle Software

This is a final team project from the Udacity online course, where we have to develop autonomous vehicle software using
the Robot Operating System (ROS). Here I developed a module to identify a traffic light using a combination of image
processing and deep learning. I developed a strategy where I trained a traffic light dataset only for detecting the
traffic light and classify the light color using a simple image processing algorithm. Having this strategy, I
successfully avoided overfitting caused by an unbalanced training data distribution, if I were to train the data using
red, yellow, green category. Moreover, pure image processing gave a more deterministic behavior of the algorithm.

After submitting the project, Udacity tested our code on their self-driving car, Carla. Our software successfully
navigates the vehicle around the test track, stopping at the red light and smoothly steering through a curve. The GIF
below shows an in-car view of our code autonomously driving Carla:

![carla](https://github.com/wlsmith42/CarND-Capstone/blob/master/imgs/carla.gif)

Udacity's feedback also included data from Carla's sensors which are shown in the GIF below:

![bag](https://github.com/wlsmith42/CarND-Capstone/blob/master/imgs/rosbag.gif)

You can find the repository in [here](https://github.com/wlsmith42/CarND-Capstone)

### Automated Fiber Placement Monitoring System
[![](http://img.youtube.com/vi/-S3dx8uJ-iA/0.jpg)](http://www.youtube.com/watch?v=-S3dx8uJ-iA "")