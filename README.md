<div align="center">
<img src="https://grow.empress.eco/uploads/default/original/2X/1/1f1e1044d3864269d2a613577edb9763890422ab.png" alt="Project Logo">
</div>

<p align="center">
WebSocket Server: a dynamic extension that supercharges real-time communication in your projects using socket.io and redis.
<br />
<a href="https://grow.empress.eco/">Explore the Docs</a>
·
<a href="https://github.com/empress-eco/websocket_server/issues">Report Bug</a>
·
<a href="https://github.com/empress-eco/websocket_server/issues">Request Feature</a>
</p>
</div>

## About The Project

WebSocket Server is a robust tool designed to supercharge your project's WebSocket server using socket.io and redis. It's the perfect choice for developers who need to manage real-time, bi-directional communication between client and server.

🌟 Key Features:
- Efficiently manage real-time communication.
- Listen to events emitted by the publish_realtime() function.
- Listen to events emitted by the client.

🛠 Built With:
- [Socket.io](https://socket.io/)
- [Redis](https://redis.io/)

This project is ideal for developers looking to enhance communication capabilities in their projects.

## Getting Started

### Prerequisites
- An existing project where you need to manage real-time communication.
- An unused port number.

### Installation

Clone the repository using the following command:

```bash
$ git clone https://github.com/empress-eco/websocket_server.git
```
Then, to add WebSocket Server to your project, use the following command:

```bash
$ bench get-app https://github.com/empress-eco/websocket_server.git
```
Next, add "fsocketio_port" key in your common_site_config.json file and set the value to an unused port number:

```json
{
  ...,
  "fsocketio_port": 9002
}
```
Add the following line in your Procfile:

```bash
fsocket_server: /usr/bin/node apps/fsocket/socketio.js
```
Running "bench start" will automatically launch a socket io server.

## Usage

WebSocket Server is easy to use. Once installed, it will automatically listen to the events emitted by the publish_realtime() function and the client. This makes managing real-time communication in your project a breeze.

## Contributing

We welcome contributions! Here's how you can contribute:

- Fork the Project
- Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
- Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
- Push to the Branch (`git push origin feature/AmazingFeature`)
- Open a Pull Request

Your contribution can make a difference. Help us enhance the WebSocket Server!

## License and Acknowledgements

### License

This project is under the MIT License. All your contributions are also licensed under the MIT License.

### Acknowledgements

Special thanks to the Empress Community, the architects behind the essential tools that power this project. Their innovation and dedication have been instrumental in building the foundations and functionalities we rely on. We are profoundly grateful for their pioneering work and ongoing support.