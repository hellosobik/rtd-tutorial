Menu Application
================

.. _installation:
Installation
------------

To use Lumache, first install it using pip:

.. code-block:: console

   (.venv) $ pip install lumache
         
.. code-block:: python
   :linenos:
   :emphasize-lines: 1

   def hello():
       print("Hello, world!")


Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :func:`lumache.get_random_ingredients`
will raise an exception.

For example:

.. code-block:: pycon

    >>> import lumache
    >>> lumache.get_random_ingredients()
    ['shells', 'gorgonzola', 'parsley']

