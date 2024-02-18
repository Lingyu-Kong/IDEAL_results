This folder contains:

- ```/init```: labeled_init.xyz, POSCAR, potential.pth ... (All the file needed for Li512 experiments)
- ```Li512.yml```: yaml file for Li512 experiments
- ```Lithium_plot.ipynb```: scripts for getting data from cloud storage and plotting

其余需要做的：

- 将Li512的实验结果打包上传清华云，实验结果包括：
    
    - 整条MD轨迹（al_serial/IDEAL-EXP-PAPER-DATA/paper_data/al_serial_Li/al_serial_Li_800/md_traj.xyz ~7GB）
    - MSD轨迹和sample_num轨迹（al_serial/IDEAL-EXP-PAPER-DATA/paper_data/plot_data_numpy/data/Li_melt/Li_800_traj.xyz）
    - RDF图的x-y数据（.npz文件，Lingyu会单独发）
    - NPT下单相法测熔点（al_serial/IDEAL-EXP-PAPER-DATA/paper_data/Li_NPT/data/*.npz, 5个npz文件）
    - 最后汇总的训练数据、最终模型、测试集数据（al_serial/IDEAL-EXP-PAPER-DATA/paper_data/Model-train-test-data/Li/total_with_bcc_bootstrap.xyz, Li_800K_val.xyz, al_serial/IDEAL-EXP-PAPER-DATA/paper_data/scripts/models/m3gnet_Li_bcc_bootstrap.pth）
    - mlff和dft弛豫结构的lattice vector对比实验数据（al_serial/IDEAL-EXP-PAPER-DATA/paper_data/relax_and_compare/results/Li_*_.xyz, 4个xyz文件）

- 说明一下百万原子多晶Li的实验数据占用内存超过了云存储限制，无法在这里提供

- 下载al_serial/IDEAL-EXP-PAPER-DATA/paper_data/plot.ipynb并重命名为Lithium_plot.ipynb发给Lingyu
