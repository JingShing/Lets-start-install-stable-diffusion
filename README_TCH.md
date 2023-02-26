[English](README.md) | 繁體中文

# 讓我們一起安裝 stable-diffusion
一篇協助安裝 stable-diffusion 的文檔

# 前置所需
* ## Python
需要 [3.10.6 版本的 Python](https://www.python.org/downloads/release/python-3106/)，安裝後記得將路徑加入系統路徑中。 Stable Diffusion Webui 會將安裝的 python 複製，再以虛擬環境安裝套件，所以不用擔心其他而外需要的套件。
* ## Git
請準備可以執行 git 指令的版本管理工具。


在安裝好 Python 和 git 後，請打開 cmd ，並執行 cd 的指令：更多有關 cd 指令的說明可以看[IBM對於CD指令說明的這一篇](https://www.ibm.com/docs/zh-tw/aix/7.1?topic=directories-changing-another-directory-cd-command)。
```bash
cd C:\path
```
上方的 path 即是你想將 Stable Diffusion Webui 安裝的資料夾路徑。建議創立名為 Stable Diffusion Webui 的資料夾，可以方便您找到此 AI 以及方便後續的更新。

在 cd 切換到正確的路徑位址後，再執行底下的指令：
```bash
git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui
```
git clone 的指令，意思是，將此網址的程式碼和檔案下載到本地的路徑中。會將 Stable Diffusion Webui 所需的程式碼都下載到前方 cd 切換的資料夾中。

後續的更新也需要 git 指令(需要先 cd 到 Stable Diffusion Webui 安裝的資料夾中，執行底下指令，即可更新)：
```bash
git pull
```

在程式碼都已經部屬到本地後，請點擊 ```webui-user.bat``` ，會下載所需要的套件，可能需要等待一段時間。全部安裝完後，即可進入 ```http://127.0.0.1:7860/```

當然，安裝結束後，只是能執行最原本的 Stable Diffusion，如果需要生成各式各樣的圖片，還是建議找適當的模型(LoRA、ckpt、safetensor)，還有適合的插件(影片、姿勢、輔助工具)。

底下是一些推薦的插件安裝和介紹文檔：
* [Ngrok](https://github.com/JingShing/Ngrok-in-StableDiffusion-tutorial/blob/main/README_TCH.md) 
  連線類，可以幫助你分享 Stable Diffusion Webui 到公網，分享給朋友或遠端使用。
* [controlNet](https://github.com/JingShing/How-to-install-controlNet/blob/main/README_TCH.md) 
  工具類，可以使用骨架生成圖片。
