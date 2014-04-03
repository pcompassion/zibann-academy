=================
 Celery Tutorial
=================


celery 의 task management
=========================

`Flower <https://github.com/mher/flower>`_
------
.. code:: bash
   celery flower --broker=redis://@localhost:6379/0 --port=


list tasks
----------

`Inspecting Workers <http://docs.celeryproject.org/en/latest/userguide/workers.html?highlight=revoke#inspecting-workers>`_

.. code:: python

   """
   """
   from celery.task.control import inspect
   
   i = inspect()

   # registered tasks
   i.registered()

   # currently executing tasks
   i.active()

   # scheduled(?)
   i.scheduled()

   # reserved: received but waiting to be executed
   i.reserved()

   
deleting pending tasks
----------------------

.. code:: bash
   $ celeryctl purge

.. code:: python

   from celery.task.control import discard_all
   discard_all()
   

kill all celery workers
-----------------------

.. code:: bash
   # `Stopping the worker <http://celery.readthedocs.org/en/latest/userguide/workers.html#stopping-the-worker>`_
   $ $ ps auxww | grep 'celery -A momsite worker' | awk '{print $2}' | xargs kill -9
