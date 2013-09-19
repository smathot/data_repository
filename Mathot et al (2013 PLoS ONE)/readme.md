Copyright 2013 Sebastiaan Mathot

Email: s.mathot@cogsci.nl

Website: http://www.cogsci.nl/smathot

About
=====

This archive contains the data described in

Mathôt, S., van der Linden, L., Grainger, J., & Vitu, F.. (2013). The pupillary light reflex reveals the focus of covert visual attention. *PLoS ONE*

License
=======

All files listed below are released under a Creative Commons Attribution-ShareAlike 3.0 Unported (CC BY-SA 3.0) license. <http://creativecommons.org/licenses/by-sa/3.0/>

Files
=====

The original .asc files, which were converted from EyeLink .edf format. They are compressed into a .tar.lzma artchive to decrease file size. These files are the ultimate source for all analyses. If you intend to do a full re-analysis of the data, you may want to start here, as the processed data elsewhere depends strongly on my own analysis path.

	data/exp1.tar.lzma
	data/exp2.tar.lzma
	
The summarized data in .csv format, one row per trial, one column per variable. In `exp1.matched.csv` all trials that couldn't be matched based on gaze deviation have been removed (see manuscript for details). Most column-names should be self-explanatory. However, you will find that the files references in the columns names `trace_[X]` are not included, because of size considerations. These files are pupil-size traces (in `.npy` format) for the various epochs, and can be regenerated from the source files above.

	data/exp1.csv
	data/exp1.matched.csv
	data/exp2.csv
	
In the `stats` folder, you will find the results from various statical analyses (prefixed with `stats.`) and numerical summaries of the data (prefixed with `summary.`).

	output/exp1/
		[Experiment 1]
		cellcount.csv
			[The number of valid trials per participant.]
		corr.csv
			[Input for the analysis shown in Fig 3a.]
		cuingVsPupilEffect.csv 
			[Cueing and pupil effect per participant, used to calculate effect sizes.]
		stats.cuingEffect.acc.csv
			[Analysis of the cueing effect in accuracy.]
		stats.cuingEffect.csv
			[Analysis of the cueing effect in RTs.]
		stats.nBlink.csv
			[Analysis of the blink rate.]
		summary.cuingEffect.acc.csv
			[Summary of the cueing effect in accuracy per participant.]
		summary.cuingEffect.csv
			[Summary of the cueing effect in RTs per participant.]
		summary.nBlink.csv
			[Summary of the blink rate per participant.]		
	output/exp2/
		[Experiment 2]
		cellcount.csv
			[The number of valid trials per participant.]
		cuingVsPupilEffect.csv
			[Cueing and pupil effect per participant, used to calculate effect sizes and for Fig 3b.]
		stats.cuingEffect.csv
			[Analysis of the cueing effect in accuracy.]
		stats.nBlink.csv
			[Analysis of the blink rate.]
		summary.cuingEffect.csv
			[Summary of the cueing effect in accuracy per participant.]
		summary.nBlink.csv
			[Summary of the blink rate per participant.]
			
The experiments are in OpenSesame format and require the `boks` and `eyelink_*` plug-ins. All these are freely available.

	experiments/exp1.opensesame.tar.gz
	experiments/exp2.opensesame.tar.gz