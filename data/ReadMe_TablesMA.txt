*************************PERCEPTION DATA*************************
alle.csv = data from perception part of experiment across all participant groups
- frist column = trialID 
- Gruppe = participant group ID (a to m), consisting of 3 participants each (1, 2, 3)

- Bewertet = participant (1/2/3) who is picking the portrayed entitiy from set of images 
		> while 1 is speaking, both 2 and 3 are picking
		> a2_w_26 = group a, person 2, female, 26 years old		

			
- Spricht = speaker portraying the entity 

- Belebtheit = German labels for animacy conditions of PORTRAYED entity
- Art = German label for animal or object subgroup of PORTRAYED entity
	> bird, mammal, reptile, appliance, vehicle, instrument
- Groesse = German label for big / small of PORTRAYED entity 
- Exemplar = German image label of PORTRAYED entitiy
- Kurz = short form of entity groups of PORTRAYED entity
		> first position: animate (belebt)/inanimate (unbelebt) = B/U
		> second position: bird (Vogel) = V / mammal (Säugetier) = S / reptile (Reptil) = r
		  appliance (Gerät) = G / vehicle (Fahrzeug) = F / instrument (Instrument) = I
		> third position: big (groß) = G / small (klein) = K

- Runde_Durchgang = round and trial within participant group
		> first position: indicates first, second or third round (one round consists of 12 trials of just one participant)
		> second position: indicates trial per round (1-12)
		> 01_04: first speaker portraying their fourth entity (within group x)
 
- Geraten_Exemplar = German image label of entity PICKED by recipients
- Geraten_Kurz = short form of entity groups of entitity PICKED by recipients
		> first position: animate (belebt)/inanimate (unbelebt) = B/U
		> second position: bird (Vogel) = V / mammal (Säugetier) = S / reptile (Reptil) = r
		  appliance (Gerät) = G / vehicle (Fahrzeug) = F / instrument (Instrument) = I
		> third position: big (groß) = G / small (klein) = K
- Geraten_Belebtheit = which animacy (Belebtheit) categroy does the picked exemplar belong to?
- Geraten_Groesse = which size (Groesse) categroy does the picked exemplar belong to?
- Geraten_Art = which nimal or object subgroup (Art) categroy does the picked exemplar belong to?


- Exemplar_Korrekt = was the intended image picked by the recipient?  (exemplar = image label)
- Gruppe_Korrekt = was the chosen exemplar of the same group (Kurz) as the portrayed entitiy?
- Belebtheit_Korrekt = was the chosen exemplar of the same animacy (Belebtheit) as the portrayed entitiy?
- Groesse_Korrekt = was the chosen exemplar of the same size (Groesse) as the portrayed entitiy?
- Art_Korrekt =  was the chosen exemplar of the same animal or object subgroup (Art) as the portrayed entitiy?



*************************PRODUCTION DATA*************************

out_praatSauce.tsv = output of praatsauce script
relevant columns:
- file = input audio file
	> a1_01_buerodrucker_m31.wav = group a, speaker 1, trial 1 (label buerodrucker), male, 31 years old
- label = vowel label 
- intervalID = interval ID across all groups and trials
- F1, F2 = forst and second formant
- A1c, A2c = apmlitude of first and second harmonic 
	   > needed for calculation of H1-H2 (A1c-A2c)
- CPP = Cepstral Peak Prominence
----------------------------------------------------------------------------------------------------------------
spectralResultsFricatives.tsv = output of praat script for analysis of fricatives by Jalal Al-Tamimi
relevant columns:
- fileName = input audio file
- phoneme = fricative label
- durationMS = duration of fricative in ms
- peakFreqHzMid =spectral peak location of fricative (highest frequency in mid 80% of phone)