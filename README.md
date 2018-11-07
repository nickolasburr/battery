# battery

`battery` is a macOS utility for analyzing battery properties.

## Installation

### Homebrew

```
brew tap nickolasburr/pfa
brew install battery
```

### Manual

Add `battery` to your `PATH` (e.g. /usr/local/bin):

```
curl -fsL https://raw.githubusercontent.com/nickolasburr/battery/master/battery > /usr/local/bin/battery
```

Make executable:

```
chmod +x /usr/local/bin/battery
```

## Options

+ `-A`, `--amperage`: Show battery amperage (in milliamps).
+ `-C`, `--is-charging`: Show whether battery potential is under capacity and in a power-gain (charging) state.
+ `-F`, `--is-fully-charged`: Show whether battery is at capacity and not in a power-gain (charging) state.
+ `-K`, `--cycle-count`: Show number of completed charge/discharge cycles.
+ `-M`, `--minutes-until-charged`: Show minutes remaining until battery is fully charged.
+ `-O`, `--minutes-until-discharged`: Show minutes remaining until battery is fully discharged.
+ `-P`, `--is-power-connected`: Show whether battery is connected to an external power source (e.g. AC power outlet).
+ `-S`, `--serial-number`: Show battery serial number.
+ `-T`, `--temperature`: Show battery temperature in Fahrenheit, Celsius, and Kelvin.
+ `-V`, `--voltage`: Show battery voltage (in millivolts).
+ `-W`, `--manufacturer`: Show battery manufacturer.

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

**Show battery temperature (in Fahrenheit, Celsius, and Kelvin)**

```shell
battery -T

# => 30.66 °C
#    87.18 °F
#    303.81 °K
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
