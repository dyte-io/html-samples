# Dyte UI Kit - HTML Samples

This repository consists of all the different ways in which you can use Dyte's
UI Kit and other packages to its full extent to get the best live audio/video
experience.

## Samples

Here are the list of available samples at the moment.

1. [Default Meeting UI](./samples/default-meeting-ui/)
2. [Using Background Transformer to modify your background](./samples/with-background-transformer/)
3. [Background Transformer UI sample](./samples/background-transformer-ui/)

## Usage

To use these samples you would need to do the following steps:

First, you'll need to create a meeting and add a participant to that meeting.

You can do so by going to https://docs.dyte.io/api?v=v2 and run the APIs in the
API runner itself so you can quickly get started.

Make sure you've created your Dyte account at https://dev.dyte.io and have your
`Organization ID` and `API Key` ready to use from the
[API Keys section](https://dev.dyte.io/apikeys).

1. Go to
   [Create Meeting API](https://docs.dyte.io/api/?v=v2#/operations/create_meeting)
   and add your credentials and run the API with your request body, note the
   `id` you receive in resonse, this is the meeting id.
2. Go to
   [Add Participant API](https://docs.dyte.io/api/?v=v2#/operations/add_participant)
   and add a participant to the meeting with the `meetingId` you received in
   previous API call.

Once you're done, you'll get an `authToken`, which you can use in a sample as
explained below.

### Trying out a sample

Here are steps to try out the samples:

1. Clone the repo:

```sh
git clone git@github.com:dyte-io/html-samples.git
cd html-samples
```

2. Install the packages with your preferred package manager and start a server,
   for example: `default-meeting-ui`.

```sh
npm install
# and to start a server
npx serve samples/default-meeting-ui
```

3. Load the server in your browser and make sure you pass the `authToken` query
   in the URL.

```
http://localhost:3000/?authToken=<your-token>
```
