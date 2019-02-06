# Jupyter on YARN

This program allows to run Jupyter on YARN with HDFS as a content manager.

# Usage

*The assumption made in Jupyter on YARN is that the machine that executes ./deploy.sh can submit jobs to the YARN cluster*

## Create an environment
./build.sh <env name>

## Deploy an environment on YARN
./deploy.sh <env name>

# Dependencies

* skein: The YARN application is described by a skein descriptor
* jupyter-omnicm: An content manager for Jupyter that supports HDFS -- Refer to this project's doc if the HDFS content management does work seamlessly 
* python3.6: the build script creates a python3.6 virtualenv (basically because I start it from a COS7 and include tensorflow in the base/requirements.txt)


