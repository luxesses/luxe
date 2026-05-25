# Systems / Low-level developer

Живу в Go, C++, Linux и Android. Пеку ML инференс на мобильных GPU, пишу сетевые демоны, автоматизирую всё что движется.

## Стек

**Языки:** Go, C, C++, Python  
**GPU:** Vulkan, Turnip Mesa, SPIR-V  
**Платформы:** Linux, Android (Magisk), macOS  
**Инструменты:** Telegram API, netlink, NDK, Ghidra

## Проекты

### [ai-node](https://github.com/menacetosociety/ai-node)
Qwen2.5 1.5B на Adreno 660 через Vulkan.  
8 tok/s на телефоне 2021 года, Telegram-бот для управления, автовосстановление после GPU crash.  
Весь инференс локально — без облаков и API ключей.

### [network-manager](https://github.com/menacetosociety/network-manager)
Изоляция устройств в WiFi сети на уровне ARP/NDP.  
Go-демон, MAC-вайтлист, управление через Telegram, watchdog.

## Как выглядит архитектура

```
Telegram → bridge (Go) → llama.cpp → Vulkan (Turnip) → Adreno 660
                    ↘ deauthd → netlink → ARP spoof
```

## Контакты

Telegram: @menace_to_society
