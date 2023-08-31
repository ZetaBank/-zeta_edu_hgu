Node configuration
====================================================

We will introduce how each sensor is organically intertwined and what function it performs.

-------------------------------------------------------------------------------

Path Planner
^^^^^^^^^^^^^^^^^^^^^^

.. thumbnail:: /_images/autodrive/18.png

- Autonomous driving control through three major sensors
- Create autonomous driving routes through Path Planner
- Consists of Global Path Planner and Local Path Planner
|

.. thumbnail:: /_images/autodrive/19.png

- Djikstra Algorithm : Provides the shortest path from one specific vertex to all other vertices
- DWA Local Planner : A path planner that plans a local path when a global path is given or a local goal is set. Used for evasive driving and bias driving.
|

-------------------------------------------------------------------------------

/scan
^^^^^^^^^^^^^^^^^^^^^^

.. thumbnail:: /_images/autodrive/20.png

- Receive scan data from LiDAR.
- Scan data is provided to perform Move base and amcl functions.
|

-------------------------------------------------------------------------------

/tf
^^^^^^^^^^^^^^^^^^^^^^

.. thumbnail:: /_images/autodrive/21.png

- Generate tf data by processing scan data with amcl algorithm
- amcl : One of the algorithms used to estimate and correct the position of the robot. Probabilistically predict the robot's position by applying a particle filter to point data input from LIDAR data.
- tf : A package that allows users to track multiple coordinate frames over time. Provides location information of coordinate frames that change over time.
|

-------------------------------------------------------------------------------

Mimetic Diagram
^^^^^^^^^^^^^^^^^^^^^^

.. thumbnail:: /_images/autodrive/22.png

- A driving plan is developed using four major types of data.
- Through this, the motor is controlled and driven.
- Receive real-time feedback on how much you moved through the encoder.
|

--------------------------------------------------------------------------------

Node Graph
^^^^^^^^^^^^^^^^^^^^^

.. thumbnail:: /_images/autodrive/23.png

|

.. thumbnail:: /_images/autodrive/24.png