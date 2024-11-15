# Sensoring malicious signal

### Privacy sensitive signals

### Malicious sensors
- acoustic
- visual
- radio

### Untrusted environments
Any devices can be planted in, can we detect them?

### Limitation of Prior Arts
- Naive pattern analysis
  - Wireless camera: Identify video traffics based on packet flow pattern, but detect video flows rather than spy cameras
  - RF Eavesdroppers: Sense RF leakage of wireless receiver circuit, detect wireless receivers rather than the eavesdroppers
 
*** Sensing invasion of signal privacy
  - audio bug recording conversation?
  - a camera watching my room?
  - wireless device decrypting my packets?

*** Stimulating + sniffing + inference
  - manipulate private signals
  - capture sensor output
  - is it responding to stimuli?

### Detect spy camera via ligh stimuli
  - video coding primer, motion compensation based compresssion, stream is divided into group of picture (GOPs)
  - stream modes: live streaming(real time, picture by picture), progressive downloading(temporarily buffered locally, transferred block by block)

### Detect eavesdropper by simulating EMR
- legitimate revceiver vs eavesdropper
- discard packet when receiver address does not match vs decode all packet

### The EarFisher System
- send some bait packets of fake receiver address
- no receiver execept eavesdropper will eat it

### Key chanllenges
- sensing memory EMR  in a crowded environment, eg, lecture room, studets wit manay electronic devices
- effectivvly stimulating eavesdropper with incurring their notice
- differentiating eavesdropper from normal memory activities

### Modeling memory EMR
- Memory access is driven by spread spectrum clock (SSC)
- Yielding a unique spectrum pattern of EMR

### Mining memory EMR under noise
- fold spectrum to search for and fuse sub-clock energy
- before and afer folding

### Separate memory EMR
- exploit clocks fingerprints to separete EMRs

### How to stimulate eavesdroppers?
- Sensing EMR nedds a large FFT windown to average noise
- Naive method:
  - stimulate using a large block of bait packets
  - but will interfere with noraml network
  - but will alert eavesdroppers

