FROM ubuntu:latest

RUN apt-get update
# If you don't have -y, Docker doesn't know what to do when the console prompts "press y to continue."
RUN apt-get install -y vim
# copies whatever that's in the first parameter (host) to the second parameter (container).
COPY ["./CopyThis", "/home"]
# Pretty much the volume option in docker run -v
VOLUME ["/home"]
ENTRYPOINT [ "/bin/bash" ]