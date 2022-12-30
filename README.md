# MTR_Interruptions

[Figma Prototype](https://www.figma.com/community/file/1190400578743283663)

## Contents

[Introduction](#introduction)

[Figma Overview](#figma-overview)

[Data Collection](#data-collection)

[Prototype Construction](#prototype-construction)

[Using the Prototype](#using-the-prototype)

## Introduction

Emergency departments (EDs) are dynamic, safety-critical environments where healthcare workers (HCWs) are interrupted as often as once every six minutes. These interruptions increase the risk of errors and preventable patient harm. As more robots enter hospitals and EDs, they must support HCWs in handling these interruptions, ideally mitigating the harmful effects of interruptions without disrupting ED communication. However, interruption-mitigation strategies are not well understood, particularly for mobile telemanipulator robots (MTRs).

We created a realistic prototype where people can simulate teleoperating a MTR in an ED. Using this prototype, we conducted a study in which ED HCWs were occasionally interrupted while using the prototype to simulate conducted patient care with an MTR. Our findings revealed insights on how MTRs might support multitasking in environments with frequent task switching, and the place of autonomy in safety-critical spaces.

Here, we describe the prototype we made and explain how to use it.

You can use the following citation or bibtex if you would like to cite this work:

S. Matsumoto, P. Ghosh, R. Jamshad, and L. D. Riek. Robot, Uninterrupted: Telemedical Robots to Mitigate Care Disruption. In Proceedings of the 2023 ACM/IEEE International Conference on Human-Robot Interaction. 2023.

Bibtex format:

```
@inproceedings{matsumoto2023Robot,
    title={Robot, Uninterrupted: Telemedical Robots to Mitigate Care Disruption},
    author={Matsumoto, Sachiko and Ghosh, Pratyusha and Jamshad, Rabeya and Riek, Laurel D.},
    booktitle={Proceedings of the 2023 ACM/IEEE International Conference on Human-Robot Interaction},
    year={2023}
}
```

## Figma Overview

Figma is a design tool that can be used to quickly prototype and test designs. In our case, we used Figma to design a control interface and interruption mitigation strategies for a MTR. We also used Figma to test our designs with ED HCWs.

If you are new to Figma, there are many tutorials you can use to learn how to use it. See some tutorials [here](https://help.figma.com/hc/en-us/sections/4405269443991-Figma-for-Beginners-4-parts-).

## Data Collection

We collected images for the Figma prototype at a medical simulation center. We reserved a room in the simulation center to record footage of the robot. The room had a patient simulator in a hospital bed and a handheld protable ultrasound, as well as various other medical equipment.

<p align="center">
<img src="https://user-images.githubusercontent.com/11902748/210017424-bca4f806-0bb9-4546-a322-78da01e45573.jpg" width=860></img>
</p>

<b>Figure 1:</b> The Stretch robot in the medical simulation center.

We used the [Stretch RE1](https://hello-robot.com/product) robot from Hello Robot in our prototype. We took the Stretch to the simulation center and mounted two GoPro cameras on top of it, near its head camera. We used GoPros because we planned to replace the head camera with a different camera, and the GoPros more closely matched the field of view and resolution we wanted. Because the GoPros were not actuated, one experimenter manually controlled the position of the GoPros during the recording.

Another experimenter teleoperated the robot in the simulation center and interacted with the patient simulator as if they were providing care for a patient. The experimenter moved the robot around the room, picked up the ultrasound probe, and pretended to administer an ultrasound on the patient simulator. All of these actions were recorded on the GoPros.

## Prototype Construction

We used the footage recorded at the simulation center to create our prototype. We extracted frames from the videos and chose frames that were approximately evenly spaced and were not blurry. We added these frames to the Figma. We iteratively designed a control interface for the robot and overlaid the interface on the frames. We then added flows in Figma between the frames so pushing a button on the interface caused the frame to change as if the robot moved. For instance, if a user clicked the button to move the robot's base forward, the frame would change as if the robot moved forward a few feet (Fig. 1).

![figma_forward](https://user-images.githubusercontent.com/11902748/210017088-0a9a7fff-e3cd-44b5-b327-5b5bf532e41c.png)
<b>Figure 1:</b> In our Figma prototype, pushing the button to move the base forward caused the frame to change as if the robot had moved forward.

## Using the Prototype
