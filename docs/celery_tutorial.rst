
celery 의 task 상황을 알아보는 법
=================================

python shell 에서
-----------------

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

   
