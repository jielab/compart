
## COMPART: Commuicable disease Modeling & Prediction Application for Research and Translation
<br/>


## 1. 准备需要的软件：
WLS (Windows subsystem for Linux)
git
cmake (sudo apt-get install cmake)
gcc (sudo apt-get install gcc)
python3 (原装或者anaconda)
Graphviz (sudo apt-get install graphviz)
doxygen (sudo apt-get install doxygen)

## 2. build covid-sim
git clone https://github.com/mrc-ide/covid-sim
cd covid-sim
mkdir build
cd build
cmake ..
cmake --build . --target all
make test
ctest

## 3. 运行测试用数据:
cd ..
./data/run_sample.py United_Kingdom

## 4. 获得论文中的报告（非常费时）
export PATH=/mnt/e/Github/covid-sim/build/src/:$PATH # or set up at ~/.bashrc
cd ./report9/GB_suppress
./runonce.sh
./batch.sh
./summariseMit.r
<br/>


### Contact & Cite

> - [Jie Huang](jiehuang001@gmail.com) MD MPH PhD, Southern University of Science and Technology
> - Manuscript under review
