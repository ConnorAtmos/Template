
## HOW TO USE THIS TEMPLATE ##


### 1. Git Clone this repository: ###

    git clone https://github.com/ConnorAtmos/Template

    or

    git clone git@github.com:ConnorAtmos/Template.git


### 2. Rename the project directory: ###

    mv Template <project_name>


### 3. CD into the project directory and remove the git repository: ###

    cd <project_name> && rm -rf .git


### 4. Run setup.py for next steps: ###

    python3 setup.py






NOTE: The following below is automatically generated. To regenerate this file, run "python3 setup.py".





This is created for Ubuntu 22.04 Check your version by running "lsb_release -a"




## HOW TO INSTALL CONDA ##


Conda is a package manager for python. It is used to install python packages and conda packages.


### 1. CD into the home directory: ###

    cd ~


### 2. Run the following command to download the conda installer: ###

    wget https://repo.anaconda.com/archive/Anaconda3-2022.05-Linux-x86_64.sh


### 3. Run the following command to install conda: ###

    bash Anaconda3-2022.05-Linux-x86_64.sh


### 4. Run the following command to update conda: ###

    conda update conda


### 5. Run the following command to install conda-forge: ###

    conda config --add channels conda-forge




## HOW TO CREATE CONDA ENVIRONMENT ##


This is for creating a new conda environment.


### 1. Run the following command to create a new conda environment: ###

    conda create --name Template


### 2. Reload the bashrc file: ###

    source ~/.bashrc

    



## HOW TO CONNECT INTERPRETER TO JETBRAINS GATEWAY ##


### 1. Open the project in PyCharm ###


### 2. Go to File > Settings > Project: Template > Python Interpreter ###


### 3. Click "Add Interpreter" > Add Local Interpreter > Conda Environment > Use Existing Environment ###


### 4. Click the drop down menu and select Template. ###




## HOW TO INSTALL REQUIREMENTS ##


This is for installing python packages and conda packages.


### 1. CD into the project directory: ###

    cd /home/connor/Template


### 2. Activate the conda environment: ###

    conda activate Template


### 3. Install the following requirements: ###

    pip install -r requirements/requirements.txt && conda install --file requirements/conda_requirements.txt  && conda install -c conda-forge --file requirements/conda_forge_requirements.txt


ALTERNATIVE, RUN THE FOLLOWING COMMAND THAT DOES ALL OF THE ABOVE:

cd /home/connor/Template && conda activate Template && pip install -r requirements/requirements.txt && conda install --file requirements/conda_requirements.txt  && conda install -c conda-forge --file requirements/conda_forge_requirements.txt




## HOW TO INSTALL SERVICE ##


A service is a program that runs in the background. This is useful for running a program that you want to run all the time, such as a web server.


### 1. Run the following command to move the service file to the correct directory: ###

    sudo mv /home/connor/Template/requirements/Template.service /etc/systemd/system/Template.service


### 2. Reload the daemon: ###

    sudo systemctl daemon-reload    


### 3. Run the following command to enable the service: ###

    sudo systemctl enable Template.service


### 4. Start the service: ###

    sudo systemctl restart Template.service


### 5. View status of service: ###

    sudo systemctl status Template.service


ALTERNATIVE, RUN THE FOLLOWING COMMAND THAT DOES ALL OF THE ABOVE:

sudo mv /home/connor/Template/requirements/Template.service /etc/systemd/system/Template.service && sudo systemctl daemon-reload && sudo systemctl enable Template.service && sudo systemctl restart Template.service && sudo systemctl status Template.service




## HOW TO UNINSTALL SERVICE ##


This is for uninstalling and removing the service.


### 1. Run the following command to disable the service: ###

    sudo systemctl disable Template.service


### 2. Run the following command to stop the service: ###

    sudo systemctl stop Template.service


### 3. Run the following command to delete the service file: ###

    sudo rm /etc/systemd/system/Template.service


ALTENATIVE, RUN THE FOLLOWING COMMAND THAT DOES ALL OF THE ABOVE:

sudo systemctl disable Template.service && sudo systemctl stop Template.service && sudo systemctl daemon-reload && sudo rm /etc/systemd/system/Template.service




## HOW TO REMOVE CONDA ENVIRONMENT ##


This is for removing the conda environment.


### 1. Run the following command to remove the conda environment: ###

    conda env remove --name Template


### 2. Reload the bashrc file: ###

    source ~/.bashrc


ALTERNATIVE, RUN THE FOLLOWING COMMAND THAT DOES ALL OF THE ABOVE:

conda env remove --name Template && source ~/.bashrc





