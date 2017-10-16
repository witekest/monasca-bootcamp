# Monasca Bootcamp, OpenStack Summit Sydney 2017

## Running the notebook on your workshop instance
---

* Download your private SSH key (monasca_workshop.pem) from
  [here](https://drive.google.com/file/d/0B799R_-18_PFYUU0eEpteTB4Mjg/view?usp=sharing)

* Set up the SSH tunnel to your instance

    * `ssh -i monasca_workshop.pem -NfL localhost:8888:localhost:8889 ubuntu@<your_instance_ip>`

* SSH to your instance and start the notebook

    * `ssh -i monasca_workshop.pem ubuntu@<your_instance_ip>`

    * `cd monasca-bootcamp`

    * `git pull`

    * `/opt/jupyter/bin/jupyter notebook --no-browser --port=8889 --notebook-dir .`

* Copy the URL and open it in your local browser. Remember to set the port number to `8888`.

* Open `Monasca Bootcamp.ipynb` notebook.

### For Windows users

* You can use your favourite SSH client

* I recommend Git BASH, BASH emulator with SSH client. (included on USB media)

## Running the notebook on your own
---
This is an iPython/Jupyter notebook that you can run on your own.
You will require:

* Ubuntu Linux 16.04

* and follow the [setup procedure](/setup/setup_procedure)
