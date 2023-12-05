You will find olympe code for anafi drone.

# Usefull command

## Setup a virtual python environnement

Launch the following command to setup a virtual python environnement for olympe build. It will allows you to avoid to change your current python environnement

```
mdkir <your_path_directory_env>
python3 -m  <your_path_directory_env>
. ./<your_path_directory_env>/bin/activate
```

You can exit this virtual environnement with the command "deactivate"

## Launch a simulation

In one window

```
sphinx "/opt/parrot-sphinx/usr/share/sphinx/drones/anafi_ai.drone"::firmware="https://firmware.parrot.com/Versions/anafi2/pc/%23latest/images/anafi2-pc.ext2.zip"
```

In antoher one

```
parrot-ue4-<biome>
```

Then, launch your python code


## Reset firmware simulation

hen you have launched an olympe python code, you should reset the firmware before launching another code.

```
sphinx-cli action -m world fwman world_reset_all
```
