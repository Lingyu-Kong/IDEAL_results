This folder contains:

- ```/init_1```: labeled_init.xyz, POSCAR, potential.pth ... (All the file needed for 1st HaberBosch experiment where we started with dissociated N2 and observed the formation of NH3)
- ```haber_bosch_1.yml```: yaml file for 1st HaberBosch experiment
- ```/init_2```: labeled_init.xyz, POSCAR, potential.pth ... (All the file needed for 2nd HaberBosch experiment where we started with N2 gas and observed the dissociation of N2)
- ```haber_bosch_2.yml```: yaml file for 2nd HaberBosch experiment
- ```Ir1000_220N2_240H2.xyz```: initial structure for the complete offline Haber Bosch MD simulation (Using the actively learned M3GNET we provide and this initial structure, there is a high probability of observing the complete Haber-Bosch reaction process at the appropriate temperature)