# TFNmodelling
Time series analysis from multiple stressors

This map contains the script and example data-set (of NW India) that is used for 
van Dijk, W.M., Densmore, A.L., Jackson, C.R., Mackay, J.D., Joshi, S.K., Sinha, R., Shekhar, S. and Gupta, S. (2019), Spatial variation of groundwater response to multiple drivers in a depleting alluvial aquifer system, northwestern India, Progress in Physical Geography, .., ..--.., DOI (DOI).

Input data consist of Input file, Observations, Calibration and Evaluation file.

%%%%%%
Input.tx includes of
Component IDs (type of time-series analysis, for published study this is 6 2 9)
6 2 9
Simulation mode (c=calibration, e=evaluation)
e
Number of runs (number of runs, more for calibration mode, Monte Carlo)
10
Objective function
1
Spin-up period
12
Acceptable model threshold (calibration only) (acceptable NSE value)
-1
Maximum number of acceptable models (calibration only)
500
Write model output files
N N Y

%%%%%%
Observations.txt includes of
NUMBER OF OBSERVATIONS
#
DAY	 MONTH	 YEAR	 RAIN	 PET	 GWL	 ABS
                   (mm/day)

%%%%%%
Calibration/IRF_Theis_calib.txt
A shape par. of climate IRF (Von Asmuth et al 2008)
min max 
b shape par. of climate IRF (a in Von Asmuth et al 2008)
0.05 0.1
n shape par. of climate IRF (a in Von Asmuth et al 2008)
0.5 2.0
f evaporation reduction factor
0.05 0.4
alpha par. of withdrawal IRF (Von Asmuth et al 2008)
0.05 1.0
gama par. of withdrawal IRF (Von Asmuth et al 2008)
1 100
Local drainage relative to a reference elevation (m)
237 238
Monthly irrigation (mm)
0.0 20.0
Canal irrigation loss coefficient
10.0 1000.0

%%%%%%
Evaluation\IRF_eval.txt (is output from calibration, file output\IRF_calib.out)
A(-)	b(-)	n(-)	f(-)	AlphaW(-)	BetaW(-)	GamaW(-)	d(m)  I(mm)	Lambda

Output is used in the paper.
