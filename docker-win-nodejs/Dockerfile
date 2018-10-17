# Use an official Windows runtime as a parent image
FROM microsoft/windowsservercore

# Configure NodeJs install
ENV NPM_CONFIG_LOGLEVEL info
ENV NODE_VERSION 8.9.4

# Install NodeJS
# Download
RUN powershell -Command "wget -Uri https://nodejs.org/dist/v%NODE_VERSION%/node-v%NODE_VERSION%-x64.msi -OutFile nodejs.msi -UseBasicParsing"

# Run the installer
RUN msiexec.exe /q /i nodejs.msi

# Install gulp-cli for runing gulp
RUN npm install -g gulp-cli

# # Set the working directory to /train
# WORKDIR /nodejs


# https://nodejs.org/dist/v8.9.4/node-v8.9.4-x64.msi