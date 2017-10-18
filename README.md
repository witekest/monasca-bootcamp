# Monasca Bootcamp, OpenStack Summit Sydney 2017

## Running the notebook on your workshop instance
---

* Download your private SSH key (monasca-bootcamp.pem) from
  [here](https://drive.google.com/open?id=0B799R_-18_PFOThSeXNiVGE4Slk)

* Set up the SSH tunnel to your instance

    * `ssh -i monasca-bootcamp.pem -NfL localhost:8889:localhost:8889 ubuntu@<your_instance_ip>`

* SSH to your instance and start the notebook

    * `ssh -i monasca-bootcamp.pem ubuntu@<your_instance_ip>`

    * `cd monasca-bootcamp`

    * `git pull`

    * `/opt/jupyter/bin/jupyter notebook --no-browser --port=8889 --notebook-dir .`

* Copy the URL and open it in your local browser.

* Open `Monasca Bootcamp.ipynb` notebook.

### For Windows users

* You can use your favourite SSH client

* I recommend Git BASH, BASH emulator with SSH client.

#### For PuTTY users

* Set the private key for authentication in `Connection -> SSH -> Auth`.
  Choose [monasca.ppk](https://drive.google.com/open?id=0B799R_-18_PFUGdIY3hXc2lxcms) as your private key.

* Add the SSH tunnel in `Connection -> SSH -> Tunnels` with:

    * `8889` as *Source port*.

    * `127.0.0.1:8889` as *Destination*.

* Remember to save the session settings.

## Running the notebook on your own
---
This is an iPython/Jupyter notebook that you can run on your own.
You will require:

* Ubuntu Linux 16.04

* and follow the [setup procedure](/setup/setup_procedure)
