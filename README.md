Bus Network Framework Comparison
================================

Help needed to complete this comparison if you are familiar with some of the technology list.

Addition of new bus network framework is welcomed.

# List of Framework

- [CAN](https://en.wikipedia.org/wiki/CAN_bus)
- [D-Bus](https://en.wikipedia.org/wiki/D-Bus)
- [DDS](https://en.wikipedia.org/wiki/Data_Distribution_Service)
- [MQTT](https://en.wikipedia.org/wiki/MQTT)
- [ZeroMQ](https://en.wikipedia.org/wiki/ZeroMQ)

# Type

|           | Type      |
|-----------|-----------|
| CAN       | Hardware  |
| D-Bus     | Software  |
| DDS       | Software  |
| MQTT      | Software  |
| ZeroMQ    | Software  |

# Broker

|           | Broker            |
|-----------|-------------------|
| CAN       | No                |
| D-Bus     | Yes               |
| DDS       | No                |
| MQTT      | Yes               |
| ZeroMQ    | Can be brokerless |

# Message Filter

|           | Message Filter    |
|-----------|-------------------|
| CAN       | Hardware or software: A filter based on CAN-ID can have dedicated hardware implementation or use software implementation. |
| D-Bus     | TODO              |
| DDS       | Topic as filter   |
| MQTT      | Topic as filter   |
| ZeroMQ    | TODO              |

# Publish/Subscribe and Request/Reply

|           | Publish/Subscribe and Request/Reply   |
|-----------|---------------------------------------|
| CAN       | Both or implementation related. Take CANopen as an example, SDO is like request/reply and PDO is like publish/subscribe.  |
| D-Bus     | TODO                                  |
| DDS       | Both                                  |
| MQTT      | Publish/Subscribe only, but request/reply can be implemented use publish/subscribe pattern.   |
| ZeroMQ    | TODO                                  |

# Implementations and License

|           | Implementations and License   |
|-----------|-------------------------------|
| CAN       | CANopenNode (Apache License 2.0), CanFestival (LGPL 2.1)  |
| D-Bus     | TODO                          |
| DDS       | RTI DDS (proprietary), eProsima Fast-DDS (Apache License 2.0), Eclipse Cyclonedds (Eclipse Public License 2.0)    |
| MQTT      | [MQTT implementations](https://en.wikipedia.org/wiki/Comparison_of_MQTT_implementations)  |
| ZeroMQ    | TODO                          |

# Security

|           | Security  |
|-----------|-----------|
| CAN       | TODO      |
| D-Bus     | TODO      |
| DDS       | TODO      |
| MQTT      | TODO      |
| ZeroMQ    | TODO      |

# Standardization

|           | Standardization       |
|-----------|-----------------------|
| CAN       | ISO 11898, CANopen, ARINC 812 or ARINC 825, DeviceNet, ISOBUS, ISO-TP, MilCAN, NMEA 2000, SAE J1939, SAE J2284, Unified Diagnostic Services (UDS), LeisureCAN |
| D-Bus     |                       |
| DDS       | OMG DDS               |
| MQTT      | OASIS MQTT, ISO 20922 |
| ZeroMQ    |                       |

# Underlying Protocol

|           | Underlying Protocol   |
|-----------|-----------------------|
| CAN       | Two wire differential signal  |
| D-Bus     | Unix domain sockets, TCP also supported.  |
| DDS       | UDP multicast if Internet is used, shared memory if on the same host. |
| MQTT      | TCP to broker         |
| ZeroMQ    | TODO                  |

# Auto Code Generation

|           | Auto code generation  |
|-----------|-----------------------|
| CAN       | Some application level standards like CANopen with stack support code generation. |
| D-Bus     |                       |
| DDS       | Yes                   |
| MQTT      | No                    |
| ZeroMQ    |                       |

# Schema in Auto Code Generation

|           | Schema in Auto Code Generation    |
|-----------|-----------------------------------|
| CAN       | Some application level standards like CANopen has EDS for code generation.    |
| D-Bus     |                                   |
| DDS       | IDL                               |
| MQTT      | No                                |
| ZeroMQ    |                                   |

# Schema Backward Compatibility

|           | Schema Backward Compatibility |
|-----------|-------------------------------|
| CAN       |                               |
| D-Bus     |                               |
| DDS       | Yes                           |
| MQTT      |                               |
| ZeroMQ    |                               |

# Programming Language Supported

|           | Programming Language Supported    |
|-----------|-----------------------------------|
| CAN       | C on most MCUs, other language is possible on embedded linux system.  |
| D-Bus     |                                   |
| DDS       | Ada, C, C#, C++, Java, Lua, Pharo, Python, Ruby, Scala    |
| MQTT      | C, C#, C++, Delphi, Erlang, Go, Haskell, Java, JavaScript, Kotlin, Lua, Pascal, Python, Ruby  |
| ZeroMQ    |                                   |

# Most Used Area

|           | Most Used Area    |
|-----------|-------------------|
| CAN       | Elevator Control System, Industrial Automation, Train Control System, Vehicle System   |
| D-Bus     | Linux Distribution Systems    |
| DDS       | Autonomous vehicles, Battleships, Dams, Financial systems, Flight systems, Medical devices, Robotics, Space systems, Train switchboard systems    |
| MQTT      | IoT               |
| ZeroMQ    |                   |

# Reliability

|           | Reliability   |
|-----------|---------------|
| CAN       |               |
| D-Bus     |               |
| DDS       |               |
| MQTT      |               |
| ZeroMQ    |               |
