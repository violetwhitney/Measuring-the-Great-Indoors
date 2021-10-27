---
moduleid: 0
title: Template as template
published: True
slug: template-template-template
---
# Sequence: Template as Template
## Sequence Summary:
This sequence of modules introduces Grasshopper as a tool-creating medium, merging concepts in HCI, spatial thinking, affordance theory to use Grasshopper as a medium for general computational design processes
## Why?
Thanks to the ecosystem of plugins, and Rhino/Grasshopper’s integration with Python/C# and other programming languages, Rhino/Grasshopper is effectively an interface/prototyping platform for spatial design and computational experimentation. Thinking and understanding of Rhino/Grasshopper as a platform, rather than a modeling program, enables us to experiment with spatial computing in conjunction with other computational tools.
## Modules:
Smart Paintbrush: Geometry as Input, Basic logic, metrics: 
Levels of Abstraction: Clusters and Plugins
Dashboards and Representation: Custom Preview, Human UI
Other Inputs: OSC, APIs, Data
Final Project: Urban Tradeoffs

Template for Modules:
===========================================

# Grasshopper as Tool-making Medium: Levels of Abstraction: Clusters and Plugins
## Module Summary

[Webhooks](https://ifttt.com/maker_webhooks) allows you to make or receive a web request with IFTTT. This means that we can get applications not already supported by IFTTT to talk to IFTTT. We will use Processing to create an HTTP request that will alert our webhook triggering an action in IFTTT. There will be three basic parts to linking IFTTT and Processing:

![blahblah](0-template-gif.gif#img-full)

- **Processing (HTTP request)** — here we can program our own unique triggers such as a button, light level, sound, number of faces in a camera can trigger our webhook. The important part is that we have all the necessary information in Processing (the API key for webhooks, and the right “event name” from webhooks.
- **Webhook (Trigger)**— when Processing triggers an HTTP request with our event name, webhooks will relay this trigger to the appropriate action based on the recipe we have created
- **IFTTT (Action)** — This can be any action from IFTTT as it normally works in IFTTT recipes.

1. sign in to [IFTTT](https://ifttt.com/home)
2. Go to `Create` → to create a new application
3. click on the **“this”** to choose our trigger. Search for **“webhooks”**. Select `webhooks` and click `connect`.

![blahblah](0-template-gif.gif#img-full)

4. Now click on the **“Receive a web request”** .
5. Create an **“Event Name”** for the trigger. I will just call mine **“turn_on”**. If you are creating a new event trigger, you should name this something unique. Then click `Create trigger`.

![blahblah](0-template-gif.gif#img-full)

6. Now we need to create our **“that”** event, click on the `that` button. Select any notification as you normally would. In our instance I will turn on an outlet from `Kasa TP-Link`.
7.Now select the Kasa TP-Link device that you plan to turn on.


