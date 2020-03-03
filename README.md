# Face Recognition ROS Wrapper
A modern ROS Wrapper for the python [face_recognition](https://github.com/ageitgey/face_recognition) library based on dlib. To get this working on your system, simply clone this repo into the `src` folder of your catkin workspace and `catkin_make`:

    cd /path/to/catkin_ws/src
    git clone https://github.com/RishabhMalviya/face_recognition_ros_wrapper.git
    cd ../
    catkin_make

## How it Works
The face_recognition algorithm needs to save encodings of known faces (as a dictionary of `name` - `encoding` pairs). When a new image appears, the system crops out faces from the new image, and compares them against the existing database using a pre-trained siamese neural network.

