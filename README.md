# Dyte UI Kit - HTML Samples

This repository consists of all the different ways in which you can use Dyte's
UI Kit and other packages to its full extent to get the best live audio/video
experience.

## Samples

Here are the list of available samples at the moment.

1. [Default Meeting UI](./samples/default-meeting-ui/)
2. [Using Background Transformer to modify your background](./samples/with-background-transformer/)

## Usage

To use these samples you would need to do the following steps:

1. Create a meeting, add a participant with our APIs
2. Use that `authToken` you receive in a sample by passing it in the URL query: `http://localhost:5173/?authToken=<your-token>`

### Trying out a sample

Here are steps to try out the samples:

1. Clone the repo:

```sh
git clone git@github.com:dyte-io/html-samples.git
```

2. Install the packages with your preferred package manager and start a server, for example: `default-meeting-ui`.

```sh
npm install
# and to start a dev server
npx serve samples/default-meeting-ui
```

3. Load the server in your browser and make sure you pass the `authToken` query in the URL.

```
http://localhost:3000/?authToken=<your-token>
```
