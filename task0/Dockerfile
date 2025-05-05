# use the latest ubuntu image as base for the image
FROM ubuntu:latest

# update the list of package in the APT repo
RUN apt-get update

# upgrade all installed packages without ask confirmation
RUN apt-get upgrade -y

# print "Hello, World!" to the terminal when the containers start
CMD ["echo", "Hello, World!"]