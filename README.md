# Info351

# Please download the work file on : [Download](https://drive.google.com/file/d/1RQZBup_yby3tJpz7ID5Deb4OuE7IEJjr/view?usp=drive_link)


# Weekly Blog 

* [Week 6](#week_6oct3---oct15)
* [Week 5](#week_5sep18---oct2)
* [Week 4](#week_4sep5---sep18)
* [Week 3](#week_3aug22---sep4) 
* [week 2](#week_2aug7---aug21)
* [Week 1](#week_1jul10---aug6)


## Week6(Oct/3 - Oct/15)

## Project View
![Game view 1](img/../image/Game_view1.PNG)
![Game View 2](img/../image/Game_vew2.PNG)

## Development Screenshots
![Overview](img/../image/Sense_1.PNG)
![Overview](img/../image/Sense_2.PNG)
![Overview](img/../image/Sense_setup.PNG)

In the development phase, I focused on creating an immersive and interactive environment. The images above showcase the progress made in designing the user interface and setting up the scene. 


## Project Achievements

- ✅ **Rough Project Completion**: I successfully completed the project, meeting the initial objectives.
- ✅ **Interaction Objects**: I implemented interaction objects within the Unity environment to enhance the user experience.
- ✅ **Switchable Senses**: Users can seamlessly switch between two senses at any time during the experience.
- ✅ **Completion on Schedule**: I managed to finish the project on time as planned.

## Areas for Improvement

While I achieved the primary objectives of the project, there are some areas where I could have done better:

- ❌ **Time Management**: I could have improved my time management skills to allocate more time to certain aspects of the project.
- ❌ **Team Collaboration**: In future projects, collaborating with a team could lead to more innovative ideas and efficient execution.

# Code view: 
<img src="img/../image/camera_change.PNG" alt="Overview" ><br>
This script in Unity allows for toggling between two cameras in a scene. It features two public camera GameObjects, "mainCamera" and "lunraCamera," and an integer "Manager" to keep track of the currently active camera.

The "ChangeCamera" function triggers a camera-switching animation, providing a smooth transition between the two cameras.

The "ManageCamera" function alternates between the cameras based on the "Manager" value. If "Manager" is 0, it activates "lunraCamera" and sets "Manager" to 1. Otherwise, it activates "mainCamera" and sets "Manager" to 0.

Two helper functions, "Cam_1" and "Cam_2," enable or disable the respective cameras based on their names.

In summary, this script facilitates camera switching in Unity, making it easy to transition between "mainCamera" and "lunraCamera" with a simple function call.



<img src="img/../image/Gun_code.PNG" alt="Overview" ><br>
This script in Unity is designed to fire bullets from a designated spawn point when an XR grab interaction is activated. It listens for the "activated" event on the XRGrabInteractable component attached to the GameObject.

When the "activated" event occurs, the "OnActivated" method is called, which in turn triggers the "FireBullet" method. This method instantiates a bullet object at the specified spawn point and gives it an initial velocity in the forward direction. The bullet is then set to self-destruct after 5 seconds.

This script is a fundamental part of implementing interactive shooting mechanics in a Unity XR project, making it possible for users to shoot bullets from a handheld object when they activate it.



# Feature Plan: 
This project is currently a work in progress and requires additional development to transform it into a fully polished game. The aim is to add various features to make it a more engaging and playable experience for users. The following requirements and enhancements are planned:
-  First Person to Third Person View Switch:
Implement the ability for players to seamlessly switch between first-person and third-person perspectives. This feature enhances gameplay and immersion.
-  Winning Condition
Introduce a winning condition or objective that players must achieve to complete the game. For example, surviving for a certain duration, completing specific tasks, or reaching a particular goal.
- Improved Weapon System
Enhance the weapon system to provide players with a more satisfying and interactive shooting experience. This may include better weapon handling, varied weapon types, and realistic ballistics.
- Non-Player Characters (NPCs)
Introduce non-player characters (NPCs) to the game world to add depth and challenges. NPCs can be allies, enemies, or neutral characters, contributing to a richer gameplay experience.
- Expanded Control Room Functionality
Expand the functionality of control rooms within the game. These control rooms may include interactive elements, puzzles, or management tasks that players must engage with to progress through the game.
## WEEK_5(Sep/18 - Oct/2)

## Current Project update: 
<img src="img/../image/Overview.PNG" alt="Overview" ><br>
<img src="img/../image/over_view2.PNG" alt="Overview" ><br>
### Over view
<img src="img/../image/game_view.PNG" alt="game_view" ><br>
### Game view

# What Have I done: 
- &#x274C; Virtual Objects 
- &#x2705; Texture feature apply 
- &#x2705; Skybox Changes 
- &#x2705; Indoor lighting 
- &#x2705; Outdoor environment changes  
- &#x2705; Simulation of weightlessness in space 

- Virtual Objects
Unfortunately, I had to abandon the virtual objects feature for now. It posed some technical challenges that needed more time to address properly.

- Texture Feature Applied
I successfully implemented a texture feature that enhances the visual quality of our project. Textures can add depth and realism to our 3D environment.

- Skybox Changes
Skyboxes play a crucial role in setting the ambiance of our scene. I've made some exciting changes to the skybox, creating different moods and atmospheres.

- Indoor Lighting
Indoor scenes now have improved lighting. Proper lighting is essential for creating a realistic and immersive environment.

- Outdoor Environment Changes
The outdoor environment has also seen significant improvements. This includes terrain modifications, vegetation, and better integration with the skybox.

- Simulation of Weightlessness in Space
One of the highlights of our project is the realistic simulation of weightlessness in space. Objects now float and move as they would in a zero-gravity environment.

# How to create Simulation of weightlessness in space: 

## Code overview: 
<img src="img/../image/code.PNG" alt="game_view" ><br>

## Code Explanation:
In the code responsible for simulating weightlessness, we use the following line as the core of the script: `transform.Rotate(_rotation * Time.deltaTime);`
  - `transform: Represents the transform component of the GameObject, which includes its position, rotation, and scale.`
  - `Rotate(): A method of the transform component used to apply a rotation.`

## Current plan: 
### Problems : 
Despite our progress, we've encountered a couple of challenges:
- 3D Environment View: When exporting the project to a new environment, we've faced issues with the 3D environment view not displaying correctly. We are actively investigating and working on solutions for this problem.
- Scale Correction: We've identified that the scale of our objects is currently too large. We plan to re-correct the scale to ensure a more realistic representation.


## Coming plan: 
### Must have: 
- Landing Space: We are working on implementing a landing space and figuring out how to transition the view from the control room to this landing area. This will also involve changes to the skybox to match the new environment.
<img src="img/../image/landing.PNG" alt="game_view" ><br>

- Door Opening Animation (Virtual): We're considering adding an animation for the door opening, enhancing the immersive experience. Alternatively, we may implement a one-button transfer mechanism for ease of use.
### Should Have: 
- We plan to introduce sound effects to the project to further immerse users. The type of sounds we'll use is still under consideration.
- Skybox Changes Button: We aim to provide users with the ability to change the skybox through a button interaction, giving them more control over the environment.
### Could have: 
- Real Object Alignments: If time allows, we may explore aligning virtual objects with real-world objects for a more seamless integration of the virtual and physical spaces.

In conclusion, our project is progressing well, but we are actively addressing some challenges and planning exciting features to enhance the experience. Stay tuned for further updates!

## WEEK_4(Sep/5 - Sep/17)
# Coming Weeks plan: 
### Must-Have: 
- Virtual Objects interaction: Create vertical button can be interacted with it.
- Texture feature apply
### Should-Have
- Actual Objects interaction
- skybox changes: environment changes by time (day and night)
## Could-Have: 
-  Indoor lighting 
-  Outdoor environment changes 
# Project Ongoing : 

### Must-Have: 
- 3D modeling (Done): This is considered essential and has been completed.
 
<img src="img/../image/sci-fi_room.png" alt="develop" ><br>
- Movement Tracking (Done): Another critical requirement that has been completed.
 <img src="img/../image/XRoginin.png" alt="develop" ><br>
- Vertical Objects interaction (Ongoing): An important feature that's currently in progress.
- Skybox changes (Ongoing): Also ongoing and important for the project.
- Texture feature apply: This is considered essential and must been completed.
 <img src="img/../image/materials.png" alt="develop" ><br>
### Should-Have:
- Actual Objects interaction - Table alignments (Planning): This is important but not as critical as the "Must-Have" items. It's in the planning stage.
- Indoor lighting (Planning): Another "Should-Have" item that's in the planning stage.
- Outdoor environment changes (Ongoing): This should enhance the project but is not essential like the "Must-Have" items.

  
### Could-Have: 
- Background story: This is considered a nice-to-have feature but not essential to the core functionality.
- Make it a game: Also a desirable but optional feature.
### Won't-Have:
- Multi-player: Explicitly excluded from the project scope.

# Potential useful rescues:  
[Black Whale Studio - XR Tutorials](https://www.youtube.com/@blackwhalestudio)
<br>
[iHeartGameDev](https://www.youtube.com/@iHeartGameDev)
# Student lecture research: 
- Inertial Measuring Unit (IMU): IMU is an electronic device that measure and reports body's specific force, angular rate, and sometime the orientation of the body, using combination of accelerometers, gyroscopes and somite magnetometers.<br> 
<img src="image/Apollo_Inertial_Measurement_Unit.png" alt="IMU" width="400" height="300">
  
- Simultaneous localization and mapping(SLAM): SLAM is the computational problem of constructing or updating a map of an unknow enviroment while simultaneously keeping track of an angent's location wihtin it.<br>
<img src="img/../image/1600px-Ouster_OS1-64_lidar_point_cloud_of_intersection_of_Folsom_and_Dore_St,_San_Francisco.png" alt="SLAM" width ="400" height="300">
  
- Outside-in motion capture for HMD’s: In outside-in systems multiple fixed external cameras are used to track the pose (3D position and 3D orientation) of the HMD. In particular, the external cameras track a set of reference points located on the headset and on the controllers (if any)

- Inside-out tracking for HMD's : Inside-Out tracking is a method of positional tracking commonly used in XR technologies, specifically for tracking the position of head-mounted displays (HMDs) and motion controller accessories.
  
# Source : 
[Inertial Measuring Unit](https://en.wikipedia.org/wiki/Inertial_measurement_unit)<br>
[Real-Time Motion Tracking for Mobile Augmented/Virtual Reality Using Adaptive Visual-Inertial Fusion](https://www.mdpi.com/1424-8220/17/5/1037)<br>
[ORB-SLAM3: An Accurate Open-Source Library for Visual, Visual–Inertial, and Multimap SLAM](https://ieeexplore.ieee.org/abstract/document/9440682)<br>
[Evaluation of the Oculus Rift S tracking system in room scale virtual reality](https://link.springer.com/article/10.1007/s10055-022-00637-3#:~:text=In%20outside%2Din%20systems%20multiple,the%20controllers%20(if%20any).)<br>
[Inside-out tracking](https://xrsi.org/definition/inside-out-tracking#:~:text=Inside%2DOut%20tracking%20is%20a,HMDs20and%20motion%20controller%20accessories.)

## WEEK_3(Aug/22 - Sep/4)

# What happened: 
Wu had some experience of 3D photogrammetry, which is transfer 2D image to 3D models. In order to make a 3D models we to take good image of the object we'd like to create 3D models, which should include basics  factory:
- Quality Camera: Utilize a high-quality camera with manual settings to capture fine details.

- Stability: Securely mount the camera on a stable platform to minimize vibrations and ensure sharp images.

- Lighting: Ensure even and diffused lighting to avoid harsh shadows or overexposed areas.

- Consistent Exposure: Keep exposure settings uniform throughout the entire photoshoot.

- Overlap: Aim for an overlap of approximately 25% to 50% between each photo. This provides enough common features for photogrammetry software to match and stitch images together.

- Fixed Perspective: Maintain a consistent height and angle for the camera throughout the capture process

## Student lecture prepare: 
Topic should include :  
- GPS: why we not using GPS in VR/AR systems
- Inertial Measuring Unit(IMU): what is IMU? why this IMU so important?
- Outside-in motion capture for HMD's: what is it? 
- inside-out tracking for HMDs: what is the different outside-int motion capture ?


## WEEK_2(Aug/7 - Aug/21)
# What Happened:
In the past two weeks, our lecture involved pairing up with fellow students to work on exciting projects. The pairs were as follows:
1. me and Mattias, we are aiming to create a space project.
2. Christine and Amelia teamed up to work on the Whack-a-mole project.
3. Andrew and Jet joined forces to tackle the Temple Run project.

During our discussions, we focused on conceptualizing our project. In the initial draft, we plan to incorporate a dashboard featuring various buttons at the top. Some of these buttons will serve functional purposes, allowing users or players to interact with the application, while others will be for navigation.

Regarding the room style, we've brainstormed several ideas and possibilities, including:
# possible dashboard:  
 - ## Minimalism: The control room style will emphasize simplicity and clean design, with a focus on essential functions and a clutter-free interface.
   <!-- ![dashboard](download.jpeg) -->
   <img src="image/download.jpeg" alt="FD" width="400" height="300">
 - ## Maximalism: The control room style will embrace complexity and a wealth of buttons and features, creating a visually rich and intricate design.
   <!-- ![dashboard](desktop-wallpaper-space-shuttle-cockpit-spaceship-cockpit.jpg) -->
    <img src="image/desktop-wallpaper-space-shuttle-cockpit-spaceship-cockpit.jpg" alt="FD" width="400" height="300">
 - ## Futurism: The control room style will embody a futuristic and avant-garde aesthetic, featuring sleek, high-tech designs, and innovative interface elements that convey a sense of forward-looking technology.
   <!-- ![dashboard](images.jpeg) -->
    <img src="image/images.jpeg" alt="FD" width="400" height="300">

# Destination
 - ## Start(moon base) :  <br>   <img src="image/moon.webp" alt="Moon" width="400" height="300">
- ## Mar :     <br> <img src="image/mar.jpeg" alt="Mar" width="400" height="300">
- ## Titan:    <br> <img src="image/titan.jpeg" alt="Titan" width="400" height="300">
- ## Saturn:    <br><img src="image/Saturn.jpeg" alt="Saturn" width="400" height="300">

# Plan: 
  - ## Stage one:(21/Aug - 25/Aug ):
    - Virtual desk
    - Room 
    - Button
    - Sky box
  - ## Stage two :(4/Sep - 15/Sep):
    - Windows animation
    - Virtual boundary set up
    - Door  
  - ## Stage three (15/Sep -- TBC):
    - Desk working with tracking
    - environment change 
  - ## Stage four (TBC):
    - If we have time to finish : 
      - Game  mechanics
      - Story
    
# What is coming: 

  - ## Student lecture:<br>
      Each of student will pick a topic relate on VR/AR technic and do a speech last 30 minutes. Each of us will need to prepare our slides and five question that will be used on our oral final exams in end of this semester. 
  - ## My Topic : <br>
      I pick the topic that are relate to tracking system. The question are : "`What are common tracking technologies to measure the position and orientation of a display device (e.g. HMD, mobile phone) in indoor and outdoor spaces. Compare range, accuracy, precision, and application scenarios.`" 
  - ## Starting Point: <br>
      In today's modern landscape, tracking technologies have become indispensable, finding extensive utility across diverse fields such as mapping, navigation, and the operation of autonomous vehicles. The Global Positioning System (GPS), a renowned tracking technology, relies on a trio of fundamental components: the 'space segment,' the 'control segment,' and the 'user segment.' Together, these constituents empower GPS to deliver remarkably precise location information anywhere on Earth.<br>Another notable example of tracking technology is exemplified by Tesla's Autopilot system. This system harnesses advanced cameras and artificial intelligence (AI) to detect and identify a wide array of objects on the road. It processes this data in real-time to make instantaneous decisions and responses, significantly enhancing vehicle safety and autonomy.

# What we learn: 
  - Empathic Computing(Mark Billinghurst):
    - Sharing Viewpoints
      - Remote Collaboration 
    - Environment Capture
      - Shared Sphere – 360 Video Sharing 
      - Multi-Scale Collaboration
      - Mini-Me
    - Emotion Recognition
    - Empathic Tele-Existence
      - Brain Synchronization
  - AUGMENTED HUMAN LAB(Suranga, Nanayakkara)
    - ASSISTIVE AUGMENTATIONS
      - Integrate
      - Enhance
      - Understand
  - Multi-sensory XR Experiences(Rob Lindeman)
    - Multi-sensory XR
    - Applied Games
    - Long-term Immersion
  - VR/AR Applications(Bruce Thomas, Mark Billinghurst):
    - Healthcare
    - Entertainment
    - Manufacturing
    - Education
    - Charity
    - Sporting
    - Military
    - Travel
  - eXtended Reality for Sports(Stefanie Zollmann):
    - XR Sport
    - Sport broadcasting
      - Snow sport tracking
      - Cricket Ball Tracking
      - on-site spectator


## WEEK_1 (Jul/10 - Aug/6)

### What have I done:<br>
In the past few weeks, our main objective has been to acquaint ourselves with various terminologies related to Virtual Reality (VR) and Augmented Reality (AR). We aimed to grasp a clear understanding of what AR, VR, XR, and MR stand for. During our lab sessions, we had the opportunity to learn from Daniel about the principles of creating an engaging game. However, the most significant milestone for us was embarking on our first 3D project. We initiated the process by working on a panoramic skybox, which served as an initial rough draft for our immersive environment. As we progress further, we look forward to refining and expanding our skills in the exciting realms of VR and AR.

In order to make a panoramic, I need to take a lot of photos.

![Raw images](image/raw_images.png)

then I need to use the Image Composite Editor to stitch those image, After few steps I got a panoramic image that looks like this.
![stitch image](image/stitch.jpg)

After I have stitch image, it's time for me to create a real skybox project. In the end my project looks like this: 

![project](image/project1.png)

### Review<br>

As beginners in 3D object creation, our progress may initially be slow due to our lack of experience in this field. However, as we delve deeper into learning about 3D technology and its tools, our growth will accelerate rapidly. Embracing the learning process and continually expanding our knowledge will lead us to create more complex and impressive 3D objects with increasing proficiency.

In general, I'm happy with my works so far so good, because this is only a start of our project and I have a lot time to work on it and try my best to improve it, if it failed my satisfiction. 

