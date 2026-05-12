# BuildCored-Orcas-Day29
SilentAssistant — BUILDCORED ORCAS Day 29

What it does. This system captures a video of your mouth, uses a vision AI to see if you are moving your lips and then has a language model generate and speak a response. It essentially acts as a silent assistant that can communicate based on visual cues without needing to type anything.

Hardware concept. The concept is a sensor-to-actuator pipeline that treats AI models like hardware components to measure glass-to-ear latency. By profiling each stage we can learn how to manage data flow and bottlenecks just like an engineer timing signals on a real embedded microchip.

What I would do differently. I'd switch from a general purpose vision model to a specialized lipreading model and run everything locally on a dedicated AI accelerator. I would also use a streaming TTS engine so the assistant starts speaking the first word while the rest of the sentence is still being generated.

Run it. python day29_starter.py
