# HomeAssistant Automatic Deadbolt Guide

## Overview

This will provide a detailed guide for configuring the deadbolt, relay, and HomeAssistant automations seen in the Roger's Tech Talk Video.

## Build of Materials

These are the components used in the Automatic Garage Door Deadbolt video:

- [Liftmaster 841LM Deadbolt](https://www.liftmaster.com/garage-door-lock/p/841LM) - [[Buy on Amazon]](https://www.amazon.com/Liftmaster-841LM-Automatic-Garage-Door/dp/B074L9JQQR)
- [MHCOZY 2 Channel 5V 12V ZigBee Smart Relay Switch](https://www.amazon.com/gp/product/B08YY7XFS3/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)
- [12V 3A Power Adapter](https://www.amazon.com/gp/product/B07XMC9D6R/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)
- [12V DC Power Jack Adapter Connectors](https://www.amazon.com/gp/product/B0B7XXH8RD/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)
- [Micro USB Cable for Relay](https://www.amazon.com/gp/product/B0BTH4NZ8M/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)
- [Junction Box for Relay](https://www.amazon.com/gp/product/B085QCT543/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&th=1)
- [ratgdo shield](https://github.com/PaulWieland/ratgdo)
- [Junction Box for ratgdo shield](https://www.amazon.com/gp/product/B0B2RHX8B3/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)

## Deadbolt

Cut the connector off from the deadbolt and expose a portion of the two wires. They will be plugged into the COM on the relay.

## Relay

Below is the wiring diagram that should be sued for the deadbolt. The relay needs to be switched to momentary interlock mode using the third phyical button on the relay. This is the button closest to the USB power connector.

![Relay Wiring Diagram](https://github.com/rogerquake/home_automation/blob/main/garage-security/deadbolt_wiring.jpg)

## HomeAssistant

Below are links to YAML files for the automations presented in the video:

- Proximity Entities
- Virtual Garage Door Button
- Deadbolt Automation
- Remote Automation


## FAQ

**- Can the Relay be Wired Multiple Ways?** The relay can technically be wired multiple ways. However, I recommend following my wiring configuration to get the same expected behavior: