# BitSecure
## Purpose
### Background
Recently, I was introduced to the concept of crypto-currency mining, and as I had a spare computer not getting much use, I decided to put it to work. Now, my mining computer spends most of it's time mining crypto-currency and doing nothing else. Because of this, I can figure out exactly what kind of network activity should be expected during normal operation, for connecting to my mining pool, updating the mining monitor, and performing a handful of other tasks. I would like the ability to track all network activity on my miner and make sure it is consistent with it's normal operation as well as identify anything unexpected.

The need for added security arises due to the unregulated nature of crypoto-currency which means that it is generated, stored, and transferred without the safety of long established financial institutions putting more of the burden on individual participants such as myself, often with a limited knowledge of network security. My goal is to use Logrythm's NetMon to monitor my own mining computer to not only ensure that my miner is running smoothly, but also gather information about what to expect and what to look out for that I can pass on to others in the crypoto-curreny community. In addition I would like provide a starting point for others concerned with securing their miners so that they can recreate my efforts and expand on it.
### Problem
BitSecure provides a convenient dashboard for visualizing network transactions that may be of interest regarding crypto-currency mining.

A computer engaged in mining may often be left on with the mining software running for days or even months on end without interruption. Because of this, the network activity often follows a predictable, repetitive pattern and any deviation may signal a issue that demands attention raging from a system failure to security breach. To address this, BitSecure features a side by side graphs for comparing current network activity against a reference chart of expected activity to make any differences in timing or data properties clearly identifiable.

On a mining computer the majority of the network traffic often takes place between a few destinations, anything out side of those destinations might be of interest, so BitSecure includes a filtered chart to list all network traffic with destinations not reached when performing baseline of normal operation. This list can then be reviewed and updated as needed.
### Solution
We started with a chart of application id by bandwidth and ran the miner to establish a baseline. As expected, the miner would send regular updates to the mining monitor and interact with the mining pool on a 5 minute interval. We then took a snapshot of the chart and included it in a markdown visualization for comparison with live network traffic. We then recorded all listed application ids for use in query for filtering out all expected applications so that we could generate a list of unexpected network traffic.
## Manifest
## Dependencies
## Setup
