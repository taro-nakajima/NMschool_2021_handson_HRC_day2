# Hands-on experiments at HRC(BL12), NM school 2021, Day 2

## Sec.1: How to align a single crystal using TOF diffraction.
### Sec. 1-1: Reciprocal lattice space.
### Sec. 1-2: TOF neutron diffraction.
### Sec. 1-3: Example of crystal alignment at HRC.
When starting a neutron scattering experiment on a single crystal at HRC, we need to know the orientation of the crystal. We measure a neutron Laue diffraction pattern with a polychromatic neutron beam (without using the Fermi chopper). A typical neutron Laue diffraction pattern is shown below.

![Run014190s](https://user-images.githubusercontent.com/50174733/144376337-cc8e8707-e416-4f50-8db9-2edfd741b45a.png)

This is a diffraction pattern for a tetragonal crystal.
* Lattice constants : a = b = 8.499 A, c = 5.528 A, alpha = beta = gamma = 90 deg.
* Space group : P-42<sub>1</sub>m
* (Nominal) horizontal scattering plane : (H,0,L)

Let us determine the orientation of the crystal from this diffraction pattern by using a web application [Neutron Laue DIffraction Pattern Simulator for HRC(BL12)](https://nakajima.issp.u-tokyo.ac.jp/tools/hrc_laue_sim/).

### Problem 1
In the latter part of this training, we will try data analysis of inelastic neutron scattering spectra of a 1D antiferromagnet CsVCl<sub>3</sub>. Before the inelastic part, let us try the alignment of the crystal.

* Preliminary info. on CsVCl<sub>3</sub>
    * Lattice constants : a = b = 7.23700 A, c = 6.02600 A, alpha = beta = 90 deg,  gamma = 120 deg.
    * Space group : P 6<sub>3</sub>/mmc
    * (Nominal) horizontal scattering plane : (H,H,L) (u=(1,1,0), v=(0,0,1))

<img width="600" alt="CsVCl3" src="https://user-images.githubusercontent.com/50174733/144379217-b996c811-c1dc-44f1-9631-f1500287977f.png">

* "scan01_Omega_-88deg.png" is the diffraction pattern measured when the Omega angle was –88 deg. (Note that there were only two detector banks when this data was measured.) The nominal orientation of the crystal was shown below.

<img width="600" alt="CsVCl3" src="https://user-images.githubusercontent.com/50174733/144383253-9293460a-315e-4efd-a289-f0b4f794dec5.png">

* Determine the orientation of the crystal using [Neutron Laue DIffraction Pattern Simulator for HRC(BL12)](https://nakajima.issp.u-tokyo.ac.jp/tools/hrc_laue_sim/).
* Once we obtained the correct orientation, we can reproduce diffraction patterns measured other orientations. For example, "scan02_Omega_-60deg.png" is the diffraction pattern measured at omega=-60 deg. Please confirm that this diffraction pattern agrees with the simulation by applying -28 deg rotation about the z axis (= omega axis). 

The crystal structures above are drawn by [VESTA](https://jp-minerals.org/vesta/jp/) program.

## Sec. 2: Spin-excitations in ferromagnets, and (1D) antiferromagnets

### Sec. 2-1: How to measure magnetic excitations of a 1D antiferromagnet

* [Accessible Q-E range of HRC(BL12)](https://nakajima.issp.u-tokyo.ac.jp/tools/hrc_qe_range/)

## Sec. 3: Finding optimum conditions for inelastic scattering measurements on CsVCl<sub>3</sub> 
### Frequency dependence of intensity and resolution

* [Flux/Resolution Simulator of HRC(BL12)](https://nakajima.issp.u-tokyo.ac.jp/tools/hrc_flux_reso_simulator/)

### Problem 2
Find optimum conditions (Chopper, orientation) to measure the magnetic excitations in CsVCl<sub>3</sub> using web apps introduced above. 

<img width="600" alt="CsVCl3" src="https://user-images.githubusercontent.com/50174733/144434020-390588be-4fdc-4b5d-9b1c-b0d76452ba41.png">

Preliminary info.
* CsVCl<sub>3</sub> exhibits 1D spin excitation along the (0,0,L) direction. 
* The dispersion relation depends only on the L index.
* The excitation energy at the Brillouin zone boundary is about 70 meV.
* There might be a small energy gap at (0,0,1).
* It would be convenient to simultaneously measure 
    * the whole dispersion relation.
    * a magnified view near (0,0,1) to see if the energy gap exists or not. 

Please make a ppt presentation in each group.
The presentation should contain
1. Chopper frequency.
2. Orientation of the crystal.
3. Accessible Q-E ranges for multiple Ei.
4. Energy resolution and intensity.


