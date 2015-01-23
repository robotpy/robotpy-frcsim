RobotPy FRCSim implementation
=============================

Provides an entrypoint that allows robot code to connect to a gazebo-based
simulation with FRCSim plugins installed.

Note: this hasn't been released yet, so it doesn't quite work in all cases!

Installation
============

Install this package using pip::

    pip3 install robotpy-frcsim

You *must* install the gazebo simulator with the instructions provided by
FIRST, which can be found at TODO.

Specifying the proper world file
================================

You need to add the 'world' keyword argument to your wpilib.run() call, with 
a path to the file to use for the world::

    if __name__ == '__main__':
        wpilib.run(MyRobot,
                   world='/usr/share/frcsim/worlds/GearsBotDemo.world')

Running your code in the simulator
==================================

Once frcsim is installed, you should be able to do this on your robot.py::

    python3 robot.py frcsim

This command will launch the simulator, simulated driver station, and your
robot code.

Examples
========

The 

Support
=======

If you think you found a bug or something that we don't support that is
supported in the other languages, file a bug at https://github.com/robotpy/robotpy-frcsim/issues

Otherwise, you can send an email to the :ref:`RobotPy mailing list <https://groups.google.com/forum/#!forum/robotpy>`_ .

Author
======

Dustin Spicuzza (dustin@virtualroadside.com)
