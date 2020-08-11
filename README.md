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

One of the applications of the online calibration was for ESG Virizon:

[![](http://img.youtube.com/vi/LgBXKWYRGc0/0.jpg)](https://www.youtube.com/watch?v=LgBXKWYRGc0 "")

### Sensor Fusion-based Multi-Sensor Calibration

Multi-Sensor Calibration combined the input of multiple sensors such as camera and LIDAR with vehicle odometry to
determine not only the orientation but also the translation of the sensors relative to the vehicle coordinate system.
I worked on the synchronization and also the filtering of the data in the software pipeline (C++) which greatly
improved the accuracy of the calibration.
Moreover, I identified the properties of the optimization algorithm used in
this application and propose some improvements to further improve the calibration accuracy.

The following is the visualization of the SLAM result from a single camera:

![sfm](https://www.all-electronics.de/wp-content/uploads/2017/05/Bild-3-Kameraposition-1024x768.png)

### Head-Up-Display Test Automation with UR10 Robot

This was one of the projects that gave me chills when I saw the result.
I developed an automated system to check the optical quality of a head-up-display. When I joined the project, the robot
could not orient itself in the room, which leads to an inaccurate measurement of the head-up-display. Later on, I
effectively identified the source of the problem by testing the system using synthetic data that I generated. In the
end, I implemented a module that enables a UR10 Robot to position the camera with a very high absolute accuracy that it
can point the optical axis of the camera into any arbitrary position in the calibration plate. I refactored the C# code
in this project almost completely to improve the robustness in the technical sense and also user interface (such as by
forcing the unit conventions). I refactored the C# code in this project to improve the robustness and
also to avoid the user's mistake (such as by forcing the unit conventions).

### Autonomous Vehicle Software

![carla](https://github.com/wlsmith42/CarND-Capstone/blob/master/imgs/carla.gif)

![bag](https://github.com/wlsmith42/CarND-Capstone/blob/master/imgs/rosbag.gif)

You can find the repository in [here](https://github.com/wlsmith42/CarND-Capstone)

### Automated Fiber Placement Monitoring System
[![](http://img.youtube.com/vi/-S3dx8uJ-iA/0.jpg)](http://www.youtube.com/watch?v=-S3dx8uJ-iA "")