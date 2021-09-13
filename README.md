# GNSS Based Context Detection

The database used for the paper "GNSS-based environmental context detection for navigation" Florent FERIOL, Damien VIVET and Yoko WATANABE.
Authors are with ISAE-SUPAERO, Université de Toulouse and ONERA


Contact: florent.feriol@isae-supaero.fr
   	 https://www.researchgate.net/profile/Florent_Feriol2

***************************************************************************************************
DATA
The four .mat files contain the gnss recordings of the Ublox EVK-M8T. The date and hour are given in the filename. All the variables are divided in 5 different messages.
If the number of samples is not the same for each messages perform a synchronization with TOW/rostime.


Each GTxxxx.csv file include the ground truth used for training with:

0: Static point (to be filtered)
1: Urban
2: Canyon
3: Trees
4: Open-sky


Each GTxxxx_test.csv file include the ground truth used for testing with the same values than for training.

*************************************************************************************************
FILTERING

As we mentioned in the article we filtered some parts of the trajectories to insure a spatial independance. Here are the coordinates for each context:

-Urban

lat_max=43.564518;
lat_min=43.564044;
long_max=1.474955;
long_min=1.4745;

-Canyon

lat_max=43.564673;
lat_min=43.564559;
long_max=1.475521;
long_min=1.475382;

-Trees 

lat_max=43.564232;
lat_min=43.563970;
long_max=1.476777;
long_min=1.476358;

-Open-sky

lat_max=43.565153;
lat_min=43.564874;
long_max=1.477229;
long_min=1.476866;
