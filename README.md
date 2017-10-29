# Monasca Bootcamp, OpenStack Summit Boston 2017

## Running the notebook on your workshop instance
---

* Copy your private key (monasca_workshop.pem) from USB media or download from
  [here](https://drive.google.com/file/d/0B799R_-18_PFYUU0eEpteTB4Mjg/view?usp=sharing)

* Set up the SSH tunnel to your instance

    * `ssh -i monasca-bootcamp.pem -NfL localhost:8888:localhost:8889 ubuntu@<your_instance_ip>`

* SSH to your instance and start the notebook

    * `ssh -i monasca-bootcamp.pem ubuntu@<your_instance_ip>`

    * `cd monasca-bootcamp`

    * `git pull`

    * `/opt/jupyter/bin/jupyter notebook --no-browser --port=8889 --notebook-dir .`

* Copy the URL and open it in your local browser. Remember to set the port number to `8888`.

* Open `MonascaBootcamp.ipynb` notebook.

### For Windows users

* You can use your favourite SSH client

* We recommend Git BASH, BASH emulator with SSH client. (included on USB media)

* Another good alternative is cmder (http://cmder.net/)

## For PuTTY users

Set the private key for authentication in Connection -> SSH -> Auth. Choose monasca.ppk as your private key.

Add the SSH tunnel in Connection -> SSH -> Tunnels with:

8889 as Source port.

127.0.0.1:8889 as Destination.

Remember to save the session settings.

### Running the notebook on your own

This is an iPython/Jupyter notebook that you can run on your own. You will require:

Ubuntu Linux 16.04

and follow the setup procedure
