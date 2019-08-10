# TFNmodelling
Time series analysis from multiple stressors

This map contains the script and example data-set (of NW India) that is used for 
van Dijk, W.M., Densmore, A.L., Jackson, C.R., Mackay, J.D., Joshi, S.K., Sinha, R., Shekhar, S. and Gupta, S. (2019), Spatial variation of groundwater response to multiple drivers in a depleting alluvial aquifer system, northwestern India, Progress in Physical Geography, .., ..--.., DOI (DOI).

Input data consist of Input file, Observations, Calibration and Evaluation file.

%%%%%%<br/>
Input.tx includes of<br/>
Component IDs (type of time-series analysis, for published study this is 6 2 9)<br/>
6 2 9<br/>
Simulation mode (c=calibration, e=evaluation)<br/>
e<br/>
Number of runs (number of runs, more for calibration mode, Monte Carlo)<br/>
10<br/>
Objective function<br/>
1<br/>
Spin-up period<br/>
12<br/>
Acceptable model threshold (calibration only) (acceptable NSE value)<br/>
-1<br/>
Maximum number of acceptable models (calibration only)<br/>
500<br/>
Write model output files<br/>
N N Y<br/>
<br/>
%%%%%%<br/>
Observations.txt includes of<br/>
NUMBER OF OBSERVATIONS<br/>
#<br/>
DAY	 MONTH	 YEAR	 RAIN	 PET	 GWL	 ABS<br/>
                   (mm/day)<br/>
<br/>
%%%%%%<br/>
Calibration/IRF_Theis_calib.txt<br/>
A shape par. of climate IRF (Von Asmuth et al 2008)<br/>
min max <br/>
b shape par. of climate IRF (a in Von Asmuth et al 2008)<br/>
0.05 0.1<br/>
n shape par. of climate IRF (a in Von Asmuth et al 2008)<br/>
0.5 2.0<br/>
f evaporation reduction factor<br/>
0.05 0.4<br/>
alpha par. of withdrawal IRF (Von Asmuth et al 2008)<br/>
0.05 1.0<br/>
gama par. of withdrawal IRF (Von Asmuth et al 2008)<br/>
1 100<br/>
Local drainage relative to a reference elevation (m)<br/>
237 238<br/>
Monthly irrigation (mm)<br/>
0.0 20.0<br/>
Canal irrigation loss coefficient<br/>
10.0 1000.0<br/>
<br/>
%%%%%%<br/>
Evaluation\IRF_eval.txt (is output from calibration, file output\IRF_calib.out)<br/>
A(-)	b(-)	n(-)	f(-)	AlphaW(-)	BetaW(-)	GamaW(-)	d(m)  I(mm)	Lambda<br/>
<br/>
Output is used in the paper.
