# System Enumeration & Security Baseline

## Scenario

An unknown laptop was provided with no documentation.
The objective was to use terminal-based techniques to identify the system,
its operating environment, and any connected devices in order to establish
a security baseline before further security analysis.

This methodology is platform-agnostic and can be applied to any computer
system (macOS, Linux, or Windows) using native OS tools.


## Objectives

- Identify the operating system, kernel, and hardware architecture
- Identify the active shell and user privilege context
- Enumerate network connectivity and exposure
- Identifying user and user privileges
- Identify physical (USB) and wireless (Bluetooth) attack surfaces
- Detect unauthorised or foreign devices that could pose a security risk

## Commands used for:

## operating system,kernel and hardware architecture 
'sw_vers'
'uname -a'

## Shell information
'echo $SHELL'
'cat /etc/shells'
'ps -p $$ -o comm='

## User & user privileges
'whoamii'
'id'

## Commands used for identifying network interface 
'ifconfig'

## Commands used for USB/Bluetooth interface Enumeration (Physical Attack Surface)
'system_profiler SPUSBDataType'
'system_profiler SPBluetoothDataType'
