# cp2k_2023
wget https://github.com/cp2k/cp2k/releases/download/v2023.1/cp2k-2023.1.tar.bz2 insted source code tar.gz
Otherwise there will errors with make
source /opt/intel/oneapi/mkl/2022.1.0/env/vars.sh
sudo ./install_requirements_ubuntu.sh 
./install_cp2k_toolchain.sh -j 16 --with-libint=no --with-openmpi=install --with-plumed=install
./install_cp2k_toolchain.sh -j 16 --with-openmpi=install --with-plumed=install
cp /home/zhangsheng/Downloads/cp2k/cp2k-2023.1/tools/toolchain/install/arch/* to the /home/zhangsheng/Downloads/cp2k/cp2k-2023.1/arch
source /home/zhangsheng/Downloads/cp2k/cp2k-2023.1/tools/toolchain/install/setup
/home/zhangsheng/Downloads/cp2k/cp2k-2023.1
make -j 16 ARCH=local VERSION="ssmp"
source /home/zhangsheng/Downloads/cp2k/cp2k-2023.1/tools/toolchain/install/setup
export PATH=/home/zhangsheng/Downloads/cp2k/cp2k-2023.1/exe/local:$PATH
export CP2K_DATA_DIR=/home/zhangsheng/Downloads/cp2k/cp2k-2023.1/data
