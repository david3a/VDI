![Screenshot](docs/images/VDI%20Logo.png)

# VDI
VDI - Virtual Digital Interconnect. Scalable real-time object processing API


VDI uses a simple model, streams are opened typically with a URL including a UUID, source write objects to the stream and readers can read sequential frames from the source or read by index to get specific frames. this allows multiple readers to access the source without conflict, readers should not attempt to modify data.

![Screenshot](docs/images/VDI%20Process%20Flow.png)

