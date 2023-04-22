# CoOS GUI Engine Workspace

CoOS GUI Engine for STM32 Workspace

## Clone

Need to clone GUI engine code together, you can clone in same time with submodule

```bash
git clone --recurse-submodules git@github.com:luswdev/coos-gui-workspace.git
```

or

```bash
git clone --recurse-submodules https://github.com/luswdev/coos-gui-workspace.git
```

## Docker Usage

All target must build in docker, to build docker image, use command below:

```bash
./docker/build.sh
```

Run docker and copy project code into container use command below:

```bash
./docker/run.sh
```

## Build Target

When in container, start build target with command:

```bash
./build.sh
```

Or it can simply done with docker execute command (run outside container):

```bash
./docker/run.sh ./build.sh
```

## Run and Test

Flash `coos-gui.bin` into STM32 MCU to run program, there is a sample of [OpenOCD](https://openocd.org/)

1. Install OpenOCD
2. Plug in stlink into your PC and attach MCU with stlink
3. Execute download.sh and wait the download progress done
4. All done!
