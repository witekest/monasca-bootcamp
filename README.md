# Monasca Bootcamp, OpenStack Summit Boston 2017

## Running the notebook on your workshop instance
---

* Copy your private key (monasca_workshop.pem) from USB media or download from
  [here](https://drive.google.com/file/d/0B799R_-18_PFYUU0eEpteTB4Mjg/view?usp=sharing)

* Set up the SSH tunnel to your instance

    * `ssh -i monasca_workshop.pem -NfL localhost:8888:localhost:8889 ubuntu@<your_instance_ip>`

* SSH to your instance and start the notebook

    * `ssh -i monasca_workshop.pem ubuntu@<your_instance_ip>`

    * `cd monasca_workshop`

    * `git pull`

    * `/opt/jupyter/bin/jupyter notebook --no-browser --port=8889 --notebook-dir .`

* Copy the URL and open it in your local browser. Remember to set the port number to `8888`.

* Open `Monasca Bootcamp.ipynb` notebook.

### For Windows users

    * You can use your favourite SSH client

    * I recommend Git BASH, BASH emulator with SSH client. (included on USB media)

### For Linux users

    * USB media is formated with exfat filesystem. You may need additional
      packages installed. E.g. for Ubuntu:

    `sudo apt-get install exfat-fuse exfat-utils`

## Running the notebook on DevStack
---
This is an iPython/Jupyter notebook that you can run on your own.
You will require the following installed on your system:

* An OpenStack DevStack VM with the Monasca DevStack plugin installed (monasca-log-api).

    * See, https://github.com/openstack/monasca-log-api/tree/master/devstack, for more details

* On DevStack VM additionally in own virtualenv:

  * Jupyter, https://jupyter.readthedocs.io/en/latest/install.html

  * python-monascaclient
