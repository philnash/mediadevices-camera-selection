# mediaDevices Camera Selection

An example of using the [mediaDevices](https://developer.mozilla.org/en-US/docs/Web/API/MediaDevices) API to choose a user's camera.

This repo now covers a couple of projects showing how to use this.

* [The basics](#basics-on-mediadevices-and-camera-selection)
* [As part of a video chat](#selecting-cameras-during-a-video-chat)

## Basics on mediaDevices and camera selection

To see how to use the API with vanilla JavaScript and a basic example. Check out the blog post on [choosing cameras in JavaScript with the `mediaDevices` API](https://www.twilio.com/blog/2018/04/choosing-cameras-javascript-mediadevices-api.html).

### See it in action

You can test the basic version of this project by [visiting it online here](https://philnash.github.io/mediadevices-camera-selection/).

### Run the project yourself

You should run this project on a local web server. I like to use [serve](https://www.npmjs.com/package/serve) for this, but you can do so as you choose.

Clone or download the repo, then change into the directory and host the files.

```bash
git clone https://github.com/philnash/mediadevices-camera-selection.git
cd mediadevices-camera-selection
```

If you want to use serve, you can install and use it with npm like so:

```bash
npm install
npm run serve
```

The page will be available at [localhost:5000/index.html](http://localhost:5000/index.html).

## Selecting cameras during a video chat

This repo contains a modified version of the [Twilio Video quickstart application](https://github.com/twilio/video-quickstart-js) with added camera selection.

### Run the project yourself

Clone or download the repo, then change into the directory and install the dependencies.

```bash
git clone https://github.com/philnash/mediadevices-camera-selection.git
cd mediadevices-camera-selection
npm install
```

Copy the `.env.template` file to `.env` and fill in the details from your [Twilio account](https://www.twilio.com/console).

Run the application with:

```bash
npm start
```

You can now view the application at [localhost:3000](http://localhost:3000). Join a room, then use the select element to change your camera. To test this with a mobile device and switch between front and back cameras, I recommend using ngrok as described below.

## Viewing on a mobile device.

If you want to test this on a mobile device, you will need to make a tunnel to your local machine. [I recommend you use ngrok for this](https://www.twilio.com/blog/2015/09/6-awesome-reasons-to-use-ngrok-when-testing-webhooks.html). You can [download and install ngrok from ngrok.com](https://ngrok.com/). Once you have it installed, run

```bash
ngrok http 5000
```

This will open a tunnel to the locally hosted project. You will get two randomly generated URLs, enter the HTTPS version into the browser in your mobile device.