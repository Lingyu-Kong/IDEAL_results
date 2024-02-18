This folder contains:

- ```/init_1```: labeled_init.xyz, POSCAR, potential.pth ... (All the file needed for HaberBosch experiments)
- ```HaberBosch_1.yml```: yaml file for HaberBosch experiments
- ```/init_2```: labeled_init.xyz, POSCAR, potential.pth ... (All the file needed for HaberBosch experiments)
- ```HaberBosch_2.yml```: yaml file for HaberBosch experiments
- ```Ir1000_220N2_240H2.xyz```: initial structure for complete offline Haber Bosch MD simulation

| _1实验和_2实验大部分一样，区别在于初始结构和温度，_1的初始结构为Ir_np.xyz或Ir_np_dense.xyz，温度为1200K，_2的初始结构为Ir1000_70H2.xyz，温度为7000K

其余需要做的：

- 将 HaberBosch 的实验结果打包上传清华云，实验结果包括：
    
    - NH3生成和N2分解的两条轨迹.xyz文件（只截取关键的反应发生的部分）
    - 最后汇总的训练数据、最终模型（al_serial/IDEAL-EXP-PAPER-DATA/paper_data/Model-train-test-data/HaberBosch/total.xyz, al_serial/IDEAL-EXP-PAPER-DATA/paper_data/scripts/models/m3gnet_HaberBosch.pth）
    - 非active learning直接deepmd导致HaberBosch反应crash掉的实验数据（al_serial/IDEAL-EXP-PAPER-DATA/paper_data/deepmd_crash/两个.xyz，一个npz文件，然后再把这个目录下的main.py改成crash_compare.py发给Lingyu）
    - 吸附能数据（al_serial/IDEAL-EXP-PAPER-DATA/paper_data/Haber_Bosch/AbsorbE_Bench/*_aimd_test.xyz）, 然后把al_serial/IDEAL-EXP-PAPER-DATA/paper_data/scripts/e_absorb.py发给我