# CSMBot - The CSM Expert
CSMBot is a LINE chatbot that knows everything about CSM. It uses OpenAI's GPT-3 model to generate responses, making it a knowledgeable and engaging companion for all CSM lovers, CSMBot is here to help!

## Setup

1. Clone this repository to your local machine.
2. Install the required Python packages with `pip install -r requirements.txt`.
3. Set your environment variables in a `.env` file in the root directory of the project. This file should include your LINE Channel Secret, LINE Channel Access Token, OpenAI API Key, and OpenAI API Base URL.

## Tutorial

For a step-by-step guide on setting up and using CSMBot, check out this [運用 Azure OpenAI 服務打造聰明的 LINE 聊天機器人 — 實作教學](https://medium.com/@ro5112/%E9%81%8B%E7%94%A8-azure-openai-%E6%9C%8D%E5%8B%99%E6%89%93%E9%80%A0%E8%81%B0%E6%98%8E%E7%9A%84-line-%E8%81%8A%E5%A4%A9%E6%A9%9F%E5%99%A8%E4%BA%BA-%E5%AF%A6%E4%BD%9C%E6%95%99%E5%AD%B8-7dfa5a8b2a50).


## Running the Bot

To run the bot locally, you need to set up a tunneling service like ngrok to expose your local server to the internet. Once you've set up ngrok or a similar service, you can run the bot with `python index_chat.py`.

Copy the temporary ngrok domain and modify your LineBot Webhook URL accordingly, which should look like this: `https://xxxx.ngrok-free.app/callback`

Verify the webook url, if the status returns success, you will be able to run the Line Chatbot. 

## Deploying to Vercel

You can deploy the bot to Vercel using the Vercel CLI or through GitHub:

### Vercel CLI

1. Install the Vercel CLI with `npm i -g vercel`.
2. Deploy the project with `vercel`.
3. Set your environment variables in the Vercel dashboard.

### GitHub

1. Push your project to a GitHub repository.
2. Log in to Vercel and go to the "Import Project" page.
3. Select "Import Git Repository" and authorize Vercel to access your GitHub account.
4. Select the repository that you want to deploy.
5. Vercel will automatically detect that you're deploying a Python project and fill in the build settings for you. If it doesn't, you can manually set the Build Command to `pip install -r requirements.txt && python index_chat.py` and the Output Directory to `.`.
6. Click "Deploy" to deploy your project.
7. Set your environment variables in the Vercel dashboard.

## Usage

Once your CSMBot is up and running, you can start using it by sending messages through the LINE app. The bot will respond with information and facts about CMS generated by the GPT-3 model. Remember, CSMBot is not a traditional chatbot, but a completion bot. It generates a continuation of the text provided to it, making the conversation more dynamic and engaging.

## Customization

CSMBot is fully customizable. You can modify the code to change how the bot responds to certain inputs, or to add new features. For example, you could add a feature that allows the bot to send images or stickers in response to certain messages.

## Contributing

Contributions to CSMBot are welcome! If you have a feature request, bug report, or proposal for improving the bot, please open an issue on GitHub. If you'd like to contribute code, please open a pull request.

## Support

If you need help with CSMBot, please open an issue on GitHub. We'll do our best to help you out.

## License

CSMBot is open source software licensed under the MIT license. See the LICENSE file for more information.

Thank you for using CSMBot! We hope you find it useful.
