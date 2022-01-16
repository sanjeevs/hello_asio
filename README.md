## Hello Asio
Try various features of boost::asio library. Using examples from boost and also a udp day time server.

## Build
For linux, source the setup.bash for setting up the env variables required for boost. I am using 1.76
For windows, create the environment variable in gui


## Building
In the build directory type the following cmds
```
cd build
cmake ..
cmake --build .
```

## Running UDP Daytime
Execute the udp server on a given port at command line
```
build/src/udp_server 1234
```

Then execute the udp client on the same port giving the sever name and port number.
```
build/src/udp_client localhost 1234
```

This should returnt the current date and time to the client.