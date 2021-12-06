
# 프로젝트명: 사고챠랑 판별머신

### 프로젝트 멤버이름및 멤버 별 소개 : 단일팀 - 정성호- 개발&발표



### 프로젝트 소개 및 개발내용

본 프로젝트는 최근들어서 카 쉐어링 시장이 발달하면서 일어나는 차량 사고와 카쉐어링 기업들의 부실한 차량관리로 인한 이용자들의 안전을 지키며 기업적입장에서는 저렴한 비용으로 차량관리를 할수 있고자 만들었습니다. 카쉐어링 이용시 차량의 사진을 업로드 하는데 이러한 부분을 이용하여 올리는 사진을 teachable machine의 머신러닝을 통하여 사고 차량인지 정상 차량인지 확인할수 있게 개발하였습니다. 

aws의 EC2를 아용하여 nginx를 활용한 웹서비스이며 google의 teachable machine 오픈소스를 이용하여 개발 하였습니다.
teachable machine 부분에서는 정상 차량의 클래스와 사고차량의 클래스를 만들었습니다.
정상 클래스에는 샘플이 대략3000개 사고 클래스에는 1000개 정도의 클래스를 주었습니다.
또한 학습은 1000번에서 25000번정도 학습 시킨 결과 3000번 이후로는 결과가 미미하였으며 샘플 사진이 정화하다면 1000번 이하의 학습에서도 정확한 결과를 보여주었습니다.
다만 이미지에 노이즈가 심하거나 차량에 이물질이 있을경우 오류를 범하는일이 있어 이러한 경우의 사진을 넣어주어 오류률을 줄였습니다 . 
아직은 소타나DN8 아반데CN7 그랜져IG페이스리프트 모델만을 적용하여 개발하였습니다. 추후에 적용차량을 추가할 계획입니다.





# Teachable Machine Community


### What is Teachable Machine?

[Teachable Machine](https://teachablemachine.withgoogle.com/) is a web-based tool that makes creating machine learning models fast, easy, and accessible for everyone. [You can try it here](https://teachablemachine.withgoogle.com/).

### Who is it for?
Educators, artists, students, innovators, makers of all kinds – really, anyone who has an idea they want to explore. No prerequisite machine learning knowledge required.

### How does it work?
You train a computer to recognize your images, sounds, and poses without writing any machine learning code. Then, use your model in your own projects, sites, apps, and more.

### What is this repository for?

This repository contains two components of [Teachable Machine](https://teachablemachine.withgoogle.com/):

1. **A [libraries](/libraries) section** that contains all of the machine learning code used in Teachable Machine. Under the hood we use [Tensorflow.js](https://www.tensorflow.org/js), a library for machine learning in Javascript, to train and run the models you make in your web browser. The `libraries` section also contains the API for [image](/libraries/image), [audio](/libraries/audio), and [pose](/libraries/pose) helper libraries that make it easier to use the models exported by Teachable Machine in your own projects.

2. **A [snippets](/snippets) section** that contains markdown snippets that are being displayed inside the export panel in [Teachable Machine](https://teachablemachine.withgoogle.com/). These snippets contain code and instructions on how to use the exported models from Teachable Machine in languages like Javascript, Java and Python.

### How can I send feedback or get in contact with you?

You have a few options:

* [Use this form](https://forms.gle/uthe2C4tZNPA11GX7).  
* Share your projects using [#teachablemachine](https://twitter.com/hashtag/teachablemachine) on Twitter or on the [Experiments with Google](https://experiments.withgoogle.com/submit) page.
* Open an issue in this repository.

## Community Contributions and Projects

* [Teachable Machine Node Library for image models](https://github.com/tr7zw/teachablemachine-node-example)
* [Teachable Machine Mobile for image models](https://github.com/mstale007/Teachable_Machine_Mobile/tree/master)


## Disclaimer

This is an experiment, not an official Google product. We’ll do our best to support and maintain this experiment but your mileage may vary.

We encourage open sourcing projects as a way of learning from each other. Please respect our and other creators’ rights, including copyright and trademark rights when present, when sharing these works and creating derivative work. If you want more info on Google's policy, you can find that [here](https://www.google.com/permissions/).
