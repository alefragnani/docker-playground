# Use an official Python runtime as a parent image
FROM microsoft/windowsservercore

# Set the working directory to /train
WORKDIR /train

# Copy the current directory contents into the container at /train
ADD /resources/train /train

# # Install any needed packages specified in requirements.txt
# RUN train

WORKDIR /script
ADD train.js /script

# make the container runnable (working gooooood)
# ENTRYPOINT [ "c:/train/train.exe" ]

# Run app.py when the container launches
# CMD ["/train/train.exe", "train.js"]

# run volume -> docker run -it --volume D:\_Fragnani\_Pessoais\GitHub\delphi-squad-demo:c:\src win-train