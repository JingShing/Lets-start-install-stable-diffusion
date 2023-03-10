English | [繁體中文](README_TCH.md)

# Lets-start-install-stable-diffusion
A repository to help you install stable diffusion

# Before Start what you need
* ## Python
You will need [Python in 3.10.6 version](https://www.python.org/downloads/release/python-3106/), after installed python you will also need to add python into system path. Stable Diffusion Webui will create a venv as a envirorment to install module it will rely on.
* ## Git
Please prepare any version git that can use git command.


After installed Python and git. Active cmd and use cd command: more instrodution for cd command can be seen in [IBM CD command](https://www.ibm.com/docs/en/aix/7.1?topic=directories-changing-another-directory-cd-command)。
```bash
cd C:\path
```
The path is the path you want to put Stable Diffusion Webui in. It is recommend to create a folder called Stable Diffusion Webui. it will be convenient for you to find this program and easily update.

after using cd turn into right folder please use the command below:
```bash
git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui
```
the meaning of git clone is to clone the code and file it need to local folder.

Update is also need to use git command(it will need to cd to the folder you installed Stable Diffusion Webui, and use the command below)：
```bash
git pull
```

After code and file cloned to the local. Active this file: ```webui-user.bat```. It will automatically download and install all the module it need and it will take some time. After all work done you can enter this url to use AI: ```http://127.0.0.1:7860/```

However, this is just the simplest Stable Diffusion. If you need to generate the image you want you might need models(LoRA、ckpt、safetensor)and appropriate extensions(videos, pose and asistent tools)。

## Extra
After all step above. If you still don't know how to use it. I will recommend you use txt2img(using text to generate image) feature. It can make you easily understand How Stable Diffusion work and how to use this tool.

Before we start using txt2img or img2img. I suggest you to get a model, which means a data set that train for AI to use and load. Models is like ckpt、safetensor、LoRA . I also suggest using ckpt and safetensor first. Here I will take [Anything v4.0](https://huggingface.co/andite/anything-v4.0/tree/main) as example. You can download this model for following step.

After get your own ckpt or safetensor. You can put it in:

```stable-diffusion-webui\models\Stable-diffusion```

![model](image/model.png)

After put the model in folder. You can restart or active your ```webui-user.bat```. After all setup done. Enter ```http://127.0.0.1:7860/``` on your browser. Then select the toppest list to load model. wait for loading. In txt2img mode. After put the prompts and parameters. You can click generate to get the image you want.

# Extensions Recommendation
Here are repositories for extensions instrodution and instruction：
* [Ngrok](https://github.com/JingShing/Ngrok-in-StableDiffusion-tutorial/blob/main/README.md) 

  It can help you share Stable Diffusion Webui on public for friends and remote use.
* [controlNet](https://github.com/JingShing/How-to-install-controlNet/blob/main/README.md) 

  It can use pose to generate images.
