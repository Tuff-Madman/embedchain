<p align="center">
  <img src="docs/logo/dark.svg" width="400px" alt="Embedchain Logo">
</p>

<p align="center">
  <a href="https://runacap.com/ross-index/q3-2023/" target="_blank" rel="noopener"><img style="width: 260px; height: 56px" src="https://runacap.com/wp-content/uploads/2023/10/ROSS_badge_black_Q3_2023.svg" alt="ROSS Index - Fastest Growing Open-Source Startups in Q3 2023 | Runa Capital" width="260" height="56"/></a>
</p>

<p align="center">
  <a href="https://pypi.org/project/embedchain/">
    <img src="https://img.shields.io/pypi/v/embedchain" alt="PyPI">
  </a>
  <a href="https://pepy.tech/project/embedchain">
    <img src="https://static.pepy.tech/badge/embedchain" alt="Downloads">
  </a>
  <a href="https://join.slack.com/t/embedchain/shared_invite/zt-22uwz3c46-Zg7cIh5rOBteT_xe1jwLDw">
    <img src="https://img.shields.io/badge/slack-embedchain-brightgreen.svg?logo=slack" alt="Slack">
  </a>
  <a href="https://discord.gg/CUU9FPhRNt">
    <img src="https://dcbadge.vercel.app/api/server/6PzXDgEjG5?style=flat" alt="Discord">
  </a>
  <a href="https://twitter.com/embedchain">
    <img src="https://img.shields.io/twitter/follow/embedchain" alt="Twitter">
  </a>
  <a href="https://colab.research.google.com/drive/138lMWhENGeEu7Q1-6lNbNTHGLZXBBz_B?usp=sharing">
    <img src="https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667" alt="Open in Colab">
  </a>
  <a href="https://codecov.io/gh/embedchain/embedchain">
    <img src="https://codecov.io/gh/embedchain/embedchain/graph/badge.svg?token=EMRRHZXW1Q" alt="codecov">
  </a>
</p>

<hr />


> ### Checkout our latest [Sadhguru AI app](https://sadhguru-ai.streamlit.app/) built using Embedchain.

## What is Embedchain?

Embedchain is an Open Source RAG Framework that makes it easy to create and deploy AI apps. At its core, Embedchain follows the design principle of being *"Conventional but Configurable"* to serve both software engineers and machine learning engineers.

Embedchain streamlines the creation of RAG applications, offering a seamless process for managing various types of unstructured data. It efficiently segments data into manageable chunks, generates relevant embeddings, and stores them in a vector database for optimized retrieval. With a suite of diverse APIs, it enables users to extract contextual information, find precise answers, or engage in interactive chat conversations, all tailored to their own data.

## 🔧 Quick install

### Python API
```bash
pip install embedchain
```

## ✨ Live demo

Checkout the [Chat with PDF](https://embedchain.ai/demo/chat-pdf) live demo we created using Embedchain. You can find the source code [here](https://github.com/embedchain/embedchain/tree/main/examples/chat-pdf).

## 🔍 Usage

<!-- Demo GIF or Image -->
<p align="center">
  <img src="docs/images/cover.gif" width="900px" alt="Embedchain Demo">
</p>

For example, you can create an Elon Musk bot using the following code:

```python
import os
from embedchain import Pipeline as App

# Create a bot instance
os.environ["OPENAI_API_KEY"] = "YOUR API KEY"
elon_bot = App()

# Embed online resources
elon_bot.add("https://en.wikipedia.org/wiki/Elon_Musk")
elon_bot.add("https://www.forbes.com/profile/elon-musk")

# Query the bot
elon_bot.query("How many companies does Elon Musk run and name those?")
# Answer: Elon Musk currently runs several companies. As of my knowledge, he is the CEO and lead designer of SpaceX, the CEO and product architect of Tesla, Inc., the CEO and founder of Neuralink, and the CEO and founder of The Boring Company. However, please note that this information may change over time, so it's always good to verify the latest updates.
```

You can also try it in your browser with Google Colab:

[![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/17ON1LPonnXAtLaZEebnOktstB_1cJJmh?usp=sharing)

## 📖 Documentation
Comprehensive guides and API documentation are available to help you get the most out of Embedchain:

- [Introduction](https://docs.embedchain.ai/get-started/introduction#what-is-embedchain)
- [Getting Started](https://docs.embedchain.ai/get-started/quickstart)
- [Examples](https://docs.embedchain.ai/examples)
- [Supported data types](https://docs.embedchain.ai/components/data-sources/overview)

## 🔗 Join the Community

Connect with fellow developers and users by joining our [Slack Workspace](https://join.slack.com/t/embedchain/shared_invite/zt-22uwz3c46-Zg7cIh5rOBteT_xe1jwLDw) or [Discord Community](https://discord.gg/CUU9FPhRNt). Dive into discussions, ask questions, and share your experiences.

## 🤝 Schedule a 1-on-1 Session

Book a [1-on-1 Session](https://cal.com/taranjeetio/ec) with the founders, to discuss any issues, provide feedback, or explore how we can improve Embedchain for you.

## 🌐 Contributing

Contributions are welcome! Please check out the issues on the repository, and feel free to open a pull request.
For more information, please see the [contributing guidelines](CONTRIBUTING.md).

For more reference, please go through [Development Guide](https://docs.embedchain.ai/contribution/dev) and [Documentation Guide](https://docs.embedchain.ai/contribution/docs).

<a href="https://github.com/embedchain/embedchain/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=embedchain/embedchain" />
</a>

## Anonymous Telemetry

We collect anonymous usage metrics to enhance our package's quality and user experience. This includes data like feature usage frequency and system info, but never personal details. The data helps us prioritize improvements and ensure compatibility. If you wish to opt-out, set the environment variable `EC_TELEMETRY=false`. We prioritize data security and don't share this data externally.

## Citation

If you utilize this repository, please consider citing it with:

```
@misc{embedchain,
  author = {Taranjeet Singh, Deshraj Yadav},
  title = {Embedchain: Data platform for LLMs - load, index, retrieve, and sync any unstructured data},
  year = {2023},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/embedchain/embedchain}},
}
```
