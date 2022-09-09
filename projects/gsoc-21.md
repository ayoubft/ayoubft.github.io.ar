# Integrating a module to 3d scan a house within the MapMint4ME android application (OSGeo - MapMint | GSoC 2021)

<center>
<img src="../img/tajine-gsoc-21.gif" alt="Tajine model uploading"/>
</center>

## Introduction of MapMint

MapMint4ME is an Android application to record your data on the field. MapMint4ME is an Android application for [MapMint](https://mapmint.com/) web-mapping services. MapMint4ME gives the users capability to store data without using the internet locally. The data can be a file stored in alpha-numeric format, an audio file, a video file or readings obtained from a Sensor Observation Service (SOS). When the user returns back to a place with network connectivity, the recorded data can be uploaded back to the server.

MapMint4ME is an android application for [MapMint](https://mapmint.com/) web-service. MapMint is an internet-based **Geographic Information System**(GIS), designed to facilitate the deployment of **Spatial Data Infrastructure**(SDI). In an SDI, geographic data, metadata, tools, and the users are connected in an interactive manner in a framework so as to use the spatial information in an efficient and flexible way.

## Abstract:

This project allows a minimalist 3D scan (taking multiple pictures, recording camera position, using opendrone map to rebuild the 3D scene) with the house faces (accessible/visible faces) then load it as georeferenced data with the database and being able to export the data back on MapMint for 3D viewing.

<center>
<a href="https://ayoubft.github.io/img/gsoc21.png" target="_blank"><img src="../img/gsoc21.png" alt="gsoc-21"/></a>
_Click the image to see full size_
</center>
## Documentation

My work consist of three parts:

### Part One: Get the pictures using MapMint4ME

- Created a [button](https://github.com/ayoubft/MapMint4ME/commit/ec347c0e5161395c31c04a7cee5a8af2bdca3c38) that direct you to the [this layout](https://github.com/ayoubft/MapMint4ME/commit/abee7d7faad96fa1ff984a517f86b543cc02f25a).
- I have created a form that can be filled with a fixed number of images taken from the mobile MapMint4ME app, and will be transfered to MapMint, here is [how to do it](https://github.com/ayoubft/Journey-GSoC-21/wiki/Create-a-FORM-in-MapMint-to-save-images-from-MapMint4ME-needed-for-3D-constructing-a-model).
- I have some issues regarding linking MapMint to MapMint4ME, so I did get the datasets for buildings from [here](https://colmap.github.io/datasets.html), and I have taken the tajjin pictures by myself.

### Part Two: Create the 3D model using ODM

- I have created a 3D model from pictures, here is the [tutorial](https://github.com/ayoubft/Journey-GSoC-21/wiki/Create-3D-scene-using-ODM).

### Part Three: Visualize the 3D model in MapMint

- Got MapMint working on virtual machine [tutorial here](https://github.com/ayoubft/Journey-GSoC-21/wiki/Setup-MapMint), then I finished up with configuring it on Docker [tutorial here](https://github.com/ayoubft/Journey-GSoC-21/wiki/Setup-MapMint-with-Docker).
- Added 3D models to the volume [see here](https://github.com/ayoubft/ZOO-Project/commit/1640b4464d1a37f747a807140f8006c121190b6f).
- Used docker [volumes](https://github.com/ayoubft/ZOO-Project/blob/docker-gsoc21/docker-compose.yml#L17-L18) to get access to the 3D models to be visualized.
- Using [threeJS](https://threejs.org/), I was able to render the 3D models in MapMint, using a [template](https://github.com/ayoubft/ZOO-Project/commit/8062585d9ec95af0a622c2f8c3ce92964621448c).

## Code Repositories:

- [ZOO-Project](https://github.com/ayoubft/ZOO-Project/tree/docker-gsoc21)
- [MapMint4ME](https://github.com/ayoubft/MapMint4ME)

## Videos:

- [Loading Models](https://drive.google.com/file/d/150PgaYOqNWTER8W0CTFqRQ4JDvy9SpLA/view?usp=sharing)

## Other Important Links:

- [Wiki on GitHub](https://github.com/ayoubft/Journey-GSoC-21/wiki)
- [Project on OSGeo Wiki](https://wiki.osgeo.org/wiki/Integrating_a_module_to_3d_scan_a_house_within_the_MapMint4ME_android_application)
