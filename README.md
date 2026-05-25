# Systems / Low-level developer

Go, C++, Linux and Android. GPU compute pipelines, network daemons, on-device ML inference, automation.

<img src="https://github-readme-stats.vercel.app/api?username=luxesses&show_icons=true&hide_title=true&count_private=true" height="150"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=luxesses&layout=compact&hide_title=true" height="150"/>

<p>
  <img src="https://img.shields.io/badge/-Go-00ADD8?style=flat&logo=go&logoColor=white"/>
  <img src="https://img.shields.io/badge/-C++-00599C?style=flat&logo=cplusplus&logoColor=white"/>
  <img src="https://img.shields.io/badge/-Vulkan-AC4142?style=flat&logo=vulkan&logoColor=white"/>
  <img src="https://img.shields.io/badge/-Android-3DDC84?style=flat&logo=android&logoColor=white"/>
  <img src="https://img.shields.io/badge/-Linux-FCC624?style=flat&logo=linux&logoColor=black"/>
  <img src="https://img.shields.io/badge/-Python-3776AB?style=flat&logo=python&logoColor=white"/>
</p>

## Projects

### [ai-node](https://github.com/luxesses/ai-node)
Qwen2.5 1.5B on Adreno 660 via Vulkan (Mesa Turnip).
8 tok/s on a 2021 phone — fully local inference, no cloud, no API keys.
Telegram bot for management, transparent GPU fault recovery.

### [network-manager](https://github.com/luxesses/network-manager)
Wireless device isolation at ARP/NDP level.
Go daemon with MAC whitelist, Telegram management, watchdog.

## Architecture

```
Telegram → bridge (Go) → llama.cpp → Vulkan (Turnip) → Adreno 660
                    ↘ network-manager → netlink → ARP spoof
```

## Contact

Telegram: @luxesses

<img src="https://github-readme-activity-graph.vercel.app/graph?username=luxesses&theme=github-light&hide_title=true" width="100%"/>
