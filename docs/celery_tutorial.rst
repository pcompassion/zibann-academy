
celery 의 task management
=========================

list tasks
----------

.. code:: python

   """
   `Inspecting Workers <http://docs.celeryproject.org/en/latest/userguide/workers.html?highlight=revoke#inspecting-workers>`_
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
   
