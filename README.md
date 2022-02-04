# Object Detector and RTSP Streamer
Use [Object Detection](https://alwaysai.co/docs/application_development/core_computer_vision_services.html#object-detection) and [RTSP Server](https://alwaysai.co/docs/edgeiq_api/video_writer.html?highlight=rtsp#edgeiq.rtsp_video_writer.RtspVideoWriter) to stream Object Detection Inference through RTSP stream. The types of objects detected can be changed by selecting different models.

## Requirements
* [alwaysAI account](https://alwaysai.co/auth?register=true)
* [alwaysAI Development Tools](https://alwaysai.co/docs/get_started/development_computer_setup.html)

## Usage
Once the alwaysAI tools are installed on your development machine (or edge device if developing directly on it) you can install and run the app with the following CLI commands:

To perform initial configuration of the app:
```
aai app configure
```

To prepare the runtime environment and install app dependencies:
```
aai app install
```

To start the app:
```
aai app start
```

To change the computer vision model, the engine and accelerator, and add additional dependencies read [this guide](https://alwaysai.co/docs/application_development/configuration_and_packaging.html).


To view the RTSP Inference stream with VLC::

        vlc -v rtsp://<device IP address>:<port>/video<stream idx>
        ex: vlc -v rtsp://122.3.0.1:5000/video0

## Support
* [Documentation](https://alwaysai.co/docs/)
* [Community Discord](https://discord.gg/z3t9pea)
* Email: support@alwaysai.co
