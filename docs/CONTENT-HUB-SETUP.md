# Content Hub Setup

The Shoppable Video Extension requires that your video is both published, transcoded and has full video metadata included. 

## Transcoding

You need a transcoding profile for your videos to be editable, and be used in your render after editing. The shoppable video extension will select the transcoding with the highest bitrate to display in the editor.

See [this page](https://amplience.com/docs/contenthub/videotranscodeprofiles.html) for more information on how to manage your transcoding profiles.

## Video Metadata

The extension uses the framerate field in the video metadata to drive frame advance controls and operations that round to the nearest frame. You'll need to make sure that this is published with the video so that the editor can access and use it. This metadata schema isn't published by default, so you might need to contact Amplience Support to add it to your account:

- Open a support ticket with [Amplience Support](https://support.amplience.com/)
- Ask for the Video Metadata Schema to be published on your Content Hub account.
- Republish any videos you want to use with the extension once it is added.

When editing, the same need to apply via your Amplience Virtual Staging Environment. See [Creating a VSE](https://amplience.com/docs/virtualstaging/creatingavse.html) for details on how to add schemas to your VSE.

Your will need to ensure that `Video` schema is added to the VSE rules for the VSE used in your Dynamic Content Hub which can be found [here](https://amplience.com/docs/development/cli-tool-examples.html#finding-the-hub-id-and-repository-id)
