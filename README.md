# Monasca Bootcamp, OpenStack Summit Boston 2017

## Running the notebook on your workshop instance
---
* Set up the SSH tunnel to your instance

    * `ssh -i monasca_workshop.pem -NfL localhost:8888:localhost:8889 ubuntu@<your_instance_ip>`

* SSH to your instance and start the notebook

    * `ssh -i monasca_workshop.pem ubuntu@<your_instance_ip>`

    * `/opt/jupyter/bin/jupyter notebook --no-browser --port=8889 --notebook-dir monasca-bootcamp/`

* Copy the URL and open it in your local browser. Remember to set the port number to `8888`.

* Open `Monasca Bootcamp.ipynb` notebook.

## Running the notebook on DevStack
---
This is an iPython/Jupyter notebook that you can run on your own.
You will require the following installed on your system:

* An OpenStack DevStack VM with the Monasca DevStack plugin installed (monasca-log-api).

    * See, https://github.com/openstack/monasca-log-api/tree/master/devstack, for more details

* On DevStack VM additionally in own virtualenv:

  * Jupyter, https://jupyter.readthedocs.io/en/latest/install.html

  * python-monascaclient
