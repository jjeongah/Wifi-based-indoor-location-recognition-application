# Wifi based indoor location recognition applicaion
 This project is for SK Planet Industry Cooperation Project (2020.8~ 2020.12)
 
## Execution environment
Windows 10, Anaconda3(admin)<br>
Anaconda3 가상환경 세팅 파일 -> environment.yaml

## Install Anaconda 3
https://www.anaconda.com/products/individual

## Import virtual environment
Anaconda Prompt에서 프로젝트 폴더로 이동 후
```
conda env create -f environment.yaml
conda env list
```
리스트에서 skplanet-wps 가상환경이 만들어졌는지 확인
```
conda activate skplanet-wps
```
가상환경 활성화


## Excute script
```
python ~.py
```
파이썬 파일(.py) - python 명령어 사용<br>
```
jupyter notebook
```
노트북 파일(.ipynb) - 명령어 실행 후 브라우저의 주피터 노트북 상에서 수정하거나<br>
혹은 vscode의 python extension 설치하면 코드 상에서 수정 가능<br>
(파이썬 kernel을 skplanet-wps으로 설정해야 함)<br>


## Steps to execte
1. Collect wifi data with collector.py
2. Put the data you want to use for model training in ml_data/signal_data
3. Run make_ml_data.ipynb (generate data for model training)
4. Train model with randomforest.ipynb and svm.ipynb (saved in ml_data folder)
5. Perform real-time recognition with detection.py


