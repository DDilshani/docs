---
layout: default
parent: MQTT
grand_parent: Communication
title: Obstacles
nav_order: 5
permalink: communication/mqtt/obstacles
---

## Obstacles Protocols
{: .no_toc }

- TOC
{:toc}


### /obstacles/?

<table>
    <tr><td>Source</td><td> GUI</td></tr>
    <tr><td>Destination</td><td> Server</td></tr>
    <tr><td>Data Type</td><td> Null</td></tr>
    <tr><td>Sample Message</td><td>
        ?
    </td></tr>
    <tr><td>Description</td><td>
        The GUI will request to send the obstacle data of the simulation environment.
    </td></tr>
</table>

### /obstacles/

<table>
    <tr><td>Source</td><td> Server </td></tr>
    <tr><td>Destination</td><td> GUI</td></tr>
    <tr><td>Data Type</td><td> JSON</td></tr>
    <tr><td>Sample Message</td><td>
        [
        Obstacle1,
        Obstacle2
        ]

    </td></tr>
    <tr><td>Description</td><td>
        The server will send this as response to the ‘{channal}/obstacles/?’ request.

        This is always a retained type message.
    </td></tr>
</table>
