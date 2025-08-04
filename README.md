# example-nodered

toolset to build single executable for Node-RED.

## Setup

- nodejs 18+
- visual studio 2022
- wixtoolset 6

```sh
# install dependencies
npm i

# build executable and installer (Windows only)
npm run build

# show outputs
ls -la ./out
ls -la ./out/en-us
```

## Usage

```sh
# launch main process
./out/nodered.bat
```

or

```sh
# install to windows service (replace xxxx to correct version)
msiexec -i ./out/en-us/example.nodered.xxxx.x64.msi

# start service
sc start example-nodered
```
