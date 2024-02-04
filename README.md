![Screenshot](docs/images/VDI%20Logo.png)


# VDI
VDI - Virtual Digital Interconnect. Scalable real-time object processing API


VDI uses a simple model, streams are opened typically with a URL including a UUID, source writes objects to the stream and readers can read sequential frames from the source or read by index to get specific frames. this allows multiple readers to access the source without conflict, readers should not attempt to modify data.

The circular buffer can be sized appropriately for the application. Typically these buffers are sized to be a power of two.

Streams are constructed with a buffer size, this has to be large enough to contain the largest object that will be written.



![Screenshot](docs/images/VDI%20Process%20Flow.png)


