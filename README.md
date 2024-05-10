# Logger
Simple logger in CPP

# How to build
```
mkdir build && cd build
cmake -S ../ -B .
make
```

# How to initialize loggger

```
Logger logger("target_log_file_name");
```

Constructor creates both .logs directory and .logs/target_log_file_name.log log file. One log file for each object. If no string was passed construtor will create .logs/common.log.

# How to log
```
logger.logInfo({});
logger.logWarning({});
logger.logError({});
logger.logDebug({});
```
