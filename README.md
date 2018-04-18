# mediaDevices Camera Selection

An example of using the [mediaDevices](https://developer.mozilla.org/en-US/docs/Web/API/MediaDevices) API to choose a user's camera.

## View the project

You should run this project on a local web server. I like to use [serve](https://www.npmjs.com/package/serve) for this, but you can do so as you choose.

Clone or download the repo, then change into the directory and host the files.

```bash
git clone https://github.com/philnash/mediadevices-camera-selection.git
cd mediadevices-camera-selection
```

If you want to use serve, you can install and use it with npm like so:

```bash
npm install
npm start
```

The page will be available at [localhost:5000/index.html](http://localhost:5000/index.html).

### Viewing on a mobile device.

If you want to test this on a mobile device, you will need to make a tunnel to your local machine. [I recommend you use ngrok for this](https://www.twilio.com/blog/2015/09/6-awesome-reasons-to-use-ngrok-when-testing-webhooks.html). You can [download and install ngrok from ngrok.com](https://ngrok.com/). Once you have it installed, run

```bash
ngrok http 5000
```

This will open a tunnel to the locally hosted project. You will get two randomly generated URLs, enter the HTTPS version into the browser in your mobile device.
