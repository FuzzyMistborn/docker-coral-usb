## Simple Docker container designed to initialize Coral TPU USB

Based on https://github.com/tnyeanderson/zet/tree/main/20240114030411

Written in order to initalize a Google Coral TPU USB device.  Annoyingly the device initially shows up with a different device ID before being initialized, which throws off USB passthrough to a VM.  This Docker image will initialize the TPU so it has the correct ID for passthrough.

https://github.com/google-coral/edgetpu/issues/536
