# GIT2019
Notes (1/1/2019)



GIT_dir: 

Each input file should start with 

GITMATLAB_path= genpath('C:\Users\pietro\Desktop\GIT_2019');
addpath(GITMATLAB_path);
GIT_dir;


The file defines the following :

%%%Cygwin Directory

git_par.dircyg = 'C:\cygwin\';

git_par.homedir = strcat(git_par.dircyg,'home\ypark\');

git_par.dirname = strcat(git_par.homedir,'TESS3.0\');

dirname=git_par.dirname;

homedir=git_par.homedir;

%datetimenow= datestr(datetime('now'),'yyyymmdd_HHMMSS');

File Descriptions: 

Examples: 

GIT_par_266nm_td : Time-dependent optimization of TESSA266

GIT_par_266nm_td_5Genesiscalls : simulation of TESSA266 with predescribed undulator. much faster.  

GIT_par_TESSO: Simulation of oscillator experiment at ANL. Uses write_recirc_field to attenuate and filter radiation field at the end of each pass and prop_spectr_recirc to refocus the radiation at the entrance of next pass oscillator. 


Core: 

GIT_fun_2019 : Uses the main script to simulate/optimize tapering by running Genesis every period


Postprocessor: 

GIT_fun_output_tindep : postorganizes the post processor for time-independent simulation

GIT_fun_output_tdep_sub : post processor for time-dependent simulation

plot_spectral_data_contour_sub : used in the above post processor to plot the spectrum 

Input files:

read_current_profile: reads current profile

readin_totalmagfile: reads magin file to write variable lat that is read in GIT_fun_2018 to read the quadrupole lattice

write_beamfile: writes the beamfile mg.beam.in; rectangular or Gaussian current distribution from current peak and length defined, 

write_beamfile_wake:  reads wake file (eloss_2.5.csv)

write_radfile: writes the radiation profile mg.rad.in





