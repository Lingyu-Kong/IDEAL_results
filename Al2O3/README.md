This folder contains:

- ```/init```: labeled_init.xyz, POSCAR, potential.pth ... (All the file needed for Al2O3_810 experiments)
- ```Al2O3.yml```: yaml file for Li512 experiments
- ```Al2O3_plot.ipynb```: scripts for getting data from cloud storage and plotting

其余需要做的：

- 将Al2O3_810的实验结果打包上传清华云，实验结果包括：
    
    - 整条MD轨迹（al_serial/IDEAL-EXP-PAPER-DATA/paper_data/al_serial_Al2O3/al_serial_Al2O3_3000/md_traj_1.xyz ~2GB, al_serial/IDEAL-EXP-PAPER-DATA/paper_data/al_serial_Al2O3/al_serial_Al2O3_9000/md_traj_2.xyz ~2GB）
    - MSD轨迹和sample_num轨迹（al_serial/IDEAL-EXP-PAPER-DATA/paper_data/plot_data_numpy/data/Al2O3_melt/Al2O3_9000_traj.xyz）
    - RDF图的x-y数据（.npz文件，Lingyu会单独发）
    - NPT下单相法测熔点（al_serial/IDEAL-EXP-PAPER-DATA/paper_data/Al2O3_NPT/data/*.npz, 5个npz文件）
    - 最后汇总的训练数据、最终模型、测试集数据（al_serial/IDEAL-EXP-PAPER-DATA/paper_data/Model-train-test-data/Al2O3/2个xyz文件, al_serial/IDEAL-EXP-PAPER-DATA/paper_data/scripts/models/m3gnet_Al2O3.pth）
    - mlff和dft弛豫结构的lattice vector对比实验数据（al_serial/IDEAL-EXP-PAPER-DATA/paper_data/relax_and_compare/results/Al2O3_*_.xyz, 2个xyz文件）

