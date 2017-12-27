# HWLogging
A Python logging wrapper with some of logging settings configured.

## Default logging settings

1. Log file name and directory to store logs.

2. Allow the log file to rollover at a predetermined size.

3. Two log outputs:

    1. console: coding debug

    2. file: application running log collection

4. Console log output shows logs which belongs to level DEBUG and above.

5. File log output stores logs which belongs to level INFO and above.

## How to use HWLogging

1. Download HWLogging

```shell
git clone https://github.com/henrywang/hwlogging.git
```

2. Import HWLogging

```Python
import hwlogging

if __name__ == "__main__":
    logger = hwlogging.Logger(__file__).logger
    logger.info("Working on file {0}.".format(__file__))
```
