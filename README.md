# Concurrent example in Erlang

This is a simple example of comunication between client and server processes in erlang

## Erlang installation

To install erlang on your machine click [here](http://joearms.github.io/installing.html]) and choose your correct distribution

## Running the code

Type erl on your console to open the erlang shell

```erlang

c(afile_server).

c(afile_client).

FileServer = afile_server:start(".").

afile_client:get_file(FileServer, "afile_server.erl").

afile_client:ls(FileServer).

```

## What the previous lines do

* The first two lines just compiles the two erlang files
* The the third line creates a Server process passing the current directory of the file server
* The fourth line the client requests a file from the server sending to it a message
* The Fifth line the client requests the list of files in the server directory sending to it a message

## Note

This is just a simple example of erlang usage, I'm a begginer! :)
