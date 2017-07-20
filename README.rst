# AWS Lambda with Python and CI

## Installation

Create virtual environment and install requirements:

.. code-block:: bash

    $ which python3.6
    /usr/local/bin/python3.6
    $ virtualenv --python $(which python3.6) venv
    $ source venv/bin/activate
    $ pip install -r requirements.txt


Configure a AWS account:

.. code-block:: bash

    $ mkdir ~/.aws
    $ cat >> ~/.aws/config
    [default]
    aws_access_key_id=YOUR_ACCESS_KEY_HERE
    aws_secret_access_key=YOUR_SECRET_ACCESS_KEY
    region=YOUR_REGION (such as us-west-2, us-west-1, etc)

  
Install Jupyter plugins

.. code-block:: bash

    $ jupyter-nbextension install rise --py --sys-prefix
    $ jupyter-nbextension enable rise --py --sys-prefix
    

Run Jupyter

.. code-block:: bash

    $ jupyter notebook