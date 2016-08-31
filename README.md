# MadEye Server

*Easily run a MadEye server*

1. [Install docker and docker-compose](https://docs.docker.com/compose/install/)
  a. If you don't want to run docker as root, you may have to add your user to the
     docker group.
2. `git clone https://github.com/mad-eye/mad-eye-server.git`
3. `cd mad-eye-server`
4. `docker-compose up`
  a. MadEye server is now running on port 80.  Make sure this is visible to the
     outside world (if you are running an EC2 instance, you'll have to configure
     your Security Groups).

*Connect to your MadEye server with the CLI*

1. Install the CLI. `curl https://madeye.io/install | sh`
2. Point to your server by setting  `export MADEYE_BASE_URL=http://XXX.XX.XX.XX` (no trailing slash)
3. Run `madeye` in your project directory

# Installing MadEye Client

`curl https://raw.githubusercontent.com/mad-eye/dementor/containerize/bin/install_madeye.sh | sh`
