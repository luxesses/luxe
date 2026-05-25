# Systems / Low-level developer

Go, C++, Linux and Android. GPU compute pipelines, network daemons, on-device ML inference, automation.

## Stack

**Languages:** Go, C, C++, Python  
**GPU:** Vulkan, Mesa Turnip, SPIR-V  
**Platforms:** Linux, Android (Magisk), macOS  
**Tools:** Telegram API, netlink, NDK, Ghidra

## Projects

### [ai-node](https://github.com/luxesses/ai-node)
Qwen2.5 1.5B on Adreno 660 via Vulkan (Mesa Turnip).  
8 tok/s on a 2021 phone — fully local, no cloud, no API keys.  
Telegram bot for management, transparent GPU fault recovery.

### [network-manager](https://github.com/luxesses/network-manager)
Wireless device isolation at ARP/NDP level.  
Go daemon with MAC whitelist, Telegram management, watchdog.

## Architecture

```
Telegram → bridge (Go) → llama.cpp → Vulkan (Turnip) → Adreno 660
                    ↘ network-manager → netlink → ARP spoof
```


