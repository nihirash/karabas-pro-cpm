# 2023.12.29
 - ZCPR is no longer blob. Sources are included
 - Autostart commands can be specified via PROFILE.SUB file
 - Any order of volumes are acceptable
 - Two SD cards are supported(implemented in compatible way with Z-Controller on ZXEvo TSConf)
 - IOByte allows switch UART outputs(dual port ZiFi), first uart will be TTY, second - UC1

# 2023.12.11
 - Memory usage optimised 
 - IDEDOS partitions work rewritten - up to 11 partitions supported
 - Example of SD Card image was added(with predefined volumes)

# Initial public version

Built with next features:
 - ADM-3A emulation on Profi's screen (85 characters per row)
 - +3E volumes as CP/M drives via Z-controller
 - ZiFi-compatible Uart accessible via IOBYTE
 - Loadable as TR-Dos binary