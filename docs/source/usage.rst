Usage
=====

.. .. _installation:

Installation
------------

To use Lumache, first install it using pip:

Prepare Helm
------------
.. code-block:: console

   (.venv) $ helm repo add zerto-z4k https://zapps-helm.zerto.com/z4k/stable

   (.venv) $ helm repo update
.. note:
   Helm name (in the example above zerto-z4k) should be a logical name entered by the user.

Obtain the Image Pull Key Secret 
--------------------------------

The image pull key secret should be used in the deployment Helm chart to enable downloading Zerto’s components images. 


.. To retrieve a list of random ingredients,
.. you can use the ``lumache.get_random_ingredients()`` function:

.. .. autofunction:: lumache.get_random_ingredients

.. The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
.. or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
.. will raise an exception.

.. .. autoexception:: lumache.InvalidKindError

.. For example:

.. >>> import lumache
.. >>> lumache.get_random_ingredients()
.. ['shells', 'gorgonzola', 'parsley']

