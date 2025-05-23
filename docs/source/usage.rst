Usage
=====

.. _installation:

Installation
------------

To use Lumache, first install it using pip:

.. code-block:: console

   (.venv) $ pip install lumache

.. code-block:: python
   :linenos:
   :hl_lines: 2,3

   def greet(name):
      print(f"Hello, {name}!")
      x=4
      y=x+2
      z=x+y
         
.. code-block:: python :hl_lines: 2,3
   def my_function(x):
       if x > 5:
           return "Greater than 5"
       else:
           return "Not greater than 5"

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

