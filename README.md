# manim-in-mac

```
# 在macOS 10.13.6上安装
conda env list
# manim
source activate manim
conda list
# python     3.7.4
# pillow     5.2.0
# opencv     3.4.2
# py-opencv  3.4.2
pip list
# pycairo    1.18.0
# pyreadline 2.1
# numpy      1.15.0
# scipy      1.1.0

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
# 安装 Homebrew

brew install cairo
brew install pkg-config
# 以上两个包无法通过pip来安装，用conda安装也有问题

# 用mactex的方式来安装latex
# http://www.tug.org/mactex/mactex-download.html

git clone https://github.com/3b1b/manim.git
```

以下是通过pip来安装：

```
conda create -n manim python=3.7
source activate manim

pip install sox
pip install ffmpeg
pip install latex
pip install pycairo
pip install -r requirements.txt
```

以下是通过conda来安装（实际的安装过程）：

```
conda env create -f environment.yml
# name: manim

pip install sox
pip install latex
```

[macOS 安装解释性数学视频的动画引擎 Manim](https://zhuanlan.zhihu.com/p/71548043)

[Manim for Mac](http://bhowell4.com/manic-install-tutorial-for-mac/)

[Learning How To Animate Videos Using manim Series – A Journey](https://talkingphysics.wordpress.com/2018/06/11/learning-how-to-animate-videos-using-manim-series-a-journey/)

[Getting Started Animating with manim and Python 3.7](https://talkingphysics.wordpress.com/2019/01/08/getting-started-animating-with-manim-and-python-3-7/)

## Using manim

Try running the following:

```
python -m manim example_scenes.py SquareToCircle -pl
```

这应该会启动 QuickTime 来运行您的示例视频。如果运行成功，初步说明manim是在正常工作。

