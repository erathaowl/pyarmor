Installation and Uninstallation
===============================

|PyArmor| is a normal Python package.  You can download the archive from PyPi_,
but it is easier to install using pip_ where is available, for example::

    pip install pyarmor

or upgrade to a newer version::

    pip install --upgrade pyarmor

There is also web ui for pyarmor, install it by this command::

    pip install pyarmor-webui

Verifying the installation
--------------------------

On all platforms, the command ``pyarmor`` should now exist on the
execution path. To verify this, enter the command::

    pyarmor --version

The result should show ``PyArmor Version X.Y.Z`` or ``PyArmor Trial Version X.Y.Z``.

If the command is not found, make sure the execution path includes the
proper directory.

Installed commands
------------------

The complete installation places these commands on the execution path:

* ``pyarmor`` is the main command. See :ref:`Using PyArmor`.

* ``pyarmor-webui`` is used to open web ui of PyArmor.

If you do not perform a complete installation (installing via
``pip``), these commands will not be installed as commands.  However,
you can still execute all the functions documented below by running
Python scripts found in the distribution folder.  The equivalent of
the ``pyarmor`` command is :file:`{pyarmor-folder}/pyarmor.py`.

``pyarmor-webui`` is :file:`{pyarmor-folder}/webui/server.py`.

Clean uninstallation
--------------------

The following files are created by `pyarmor` after it has been installed::

    ~/.pyarmor/.pyarmor_capsule.zip    (since v6.2.0)
    ~/.pyarmor/license.lic             (since v5.8.0)
    ~/.pyarmor/platforms/

    {pyarmor-folder}/license.lic       (before v5.8.0)
    ~/.pyarmor_capsule.zip             (before v6.2.0)

    /path/to/project/.pyarmor_config   (if using project)

Run the following commands to make a clean uninstallation::

    pip uninstall pyarmor

    rm -rf ~/.pyarmor
    rm -rf {pyarmor-folder}            (before v5.8.0)
    rm -rf ~/.pyarmor_capsule.zip      (before v6.2.0)

    rm /path/to/project/.pyarmor_config

.. note::

   The path ``~`` may be different when logging by different user.

.. include:: _common_definitions.txt
