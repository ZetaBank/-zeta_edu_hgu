Automatic Charging 
====================================================

Description of components and algorithms required for automatic charging

-------------------------------------------------------------------------------

Component
^^^^^^^^^^^^^^^^^^^^^^

.. thumbnail:: /_images/autocharge/part.png

- Consisting of robot and station
- A system that is charged by combining the charging terminal and the docking part of the station
|

.. thumbnail:: /_images/autocharge/part2.png

|

---------------------------------------------------------------------------------------

Process
^^^^^^^^^^^^^^^^

.. raw:: html

    <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe src="https://youtube.com/embed/j11D6wvbykc?si=ctEwIxzU2JO6k73D" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
    </div>

|

1. Move to specified charging coordinates
2. Rotate to check station position
3. Move the robot so that the station is located in the exact center of the robot.
4. After confirming that it is located in the center, perform the docking process.
5. 1 second after the click sound, the LED color changes to match the robot battery status.