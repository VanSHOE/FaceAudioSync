# Image-Audio Lip Sync
### Introduction
This project takes in an image and an audio file and maps the audio to the image, creating a lip-synced video. It utilizes two existing open-source repositories: [Wav2Lip](https://github.com/Rudrabha/Wav2Lip) for audio-to-video lip syncing and [One-Shot Free-View Neural Talking-Head Synthesis](https://github.com/zhanglonghao1992/One-Shot_Free-View_Neural_Talking_Head_Synthesis) for generating a video from a single image.

This tool can be useful for a variety of applications, such as creating realistic talking head videos for presentations or video production, or for generating lip-synced animations in real-time applications. The process involves running the audio and image through each repository, combining the resulting video to generate the final output. The resulting image can be saved or further processed as needed.

Here is a video showcasing it in action: 

[![DEMO](https://img.youtube.com/vi/Ya2XJZz7N8w/0.jpg)](https://www.youtube.com/watch?v=Ya2XJZz7N8w) 

Template for frontend: https://berrydashboard.io/

### Usage 

To use this tool, follow the steps below:

1. Open the hamburger menu on the application interface.
2. Click on the "Upload Media" button to select and upload your image and audio files.
3. Once you have selected your files, click on the "Send" button to submit the data.
4. The data will be sent to the Node.js backend, which will further send it to a server running a heavy-duty GPU for processing.
5. After the processing is complete, the final data will be sent back to the application interface.

Please note that the processing time may vary depending on the size and complexity of the files, as well as the availability of the GPU server. You can monitor the progress of your request in the application interface, and the final output will be displayed once the processing is complete.

For more detailed instructions on how to set up and configure this tool, please refer to the "Installation" and "Configuration" sections of this README file.

### Installation
The deployed version of this server already exists at: mernvendorbuyer.me
#### Frontend
To install the frontend of this tool, simply clone the repository and run the following command:
`yarn ; ./deploy.sh`

#### Backend
To install and run the backend, navigate to the backend directory and run the following command:

`yarn ; node server.js`

Please note that in order to use the tool, you will also need to set up a separate server with a heavy-duty GPU for processing. This server should be specified in the backend/server.js file.

Additionally, it is recommended to set up SSL for the backend and frontend server in order to avoid browser warnings and blockages. Please refer to the appropriate SSL documentation for your server and configuration.
