# battery

`battery` is a CLI for analyzing information about your MacBook (Pro) battery.

## Installation

### Homebrew

```
brew tap nickolasburr/pfa
brew install battery
```

### Manual

Add the file to your PATH (e.g. /usr/local/bin):

```
cd /usr/local/bin && curl -sSL -O https://raw.githubusercontent.com/nickolasburr/battery/master/battery
```

Make it executable:

```
# /usr/local/bin
chmod 755 battery
```

## Options

+ `--amperage`, `-A`: Show battery amperage (in milliamps).
+ `--is-charging`, `-C`: Show whether battery potential is under capacity and in a power-gain (charging) state.
+ `--is-fully-charged`, `-F`: Show whether battery is at capacity and not in a power-gain (charging) state.
+ `--cycle-count`, `-K`: Show number of completed charge/discharge cycles.
+ `--minutes-until-charged`, `-M`: Show minutes remaining until battery is fully charged.
+ `--minutes-until-discharged`, `-O`: Show minutes remaining until battery is fully discharged.
+ `--is-power-connected`, `-P`: Show whether battery is connected to an external power source (e.g. AC power outlet).
+ `--serial-number`, `-S`: Show battery serial number.
+ `--temperature`, `-T`: Show battery temperature in Fahrenheit, Celsius, and Kelvin.
+ `--voltage`, `-V`: Show battery voltage (in millivolts).
+ `--manufacturer`, `-W`: Show battery manufacturer.

## Examples

**Show battery amperage**

```shell
battery -A
# => 673mA
```

**Show the number of completed charge/discharge cycles**

```shell
battery -K
# => 249
```

**Show minutes until battery is fully discharged**

```shell
battery -O
# => 35
```

**Show if the battery is connected to a power source**

```shell
battery -P
# => false
```

**Show battery serial number**

```shell
battery -S
# => E93VG22TC81H0B1F3
```

**Show battery voltage**

```shell
battery -V
# => 12375mV
```

**Show battery manufacturer**

```shell
battery -W
# => SMP
```
