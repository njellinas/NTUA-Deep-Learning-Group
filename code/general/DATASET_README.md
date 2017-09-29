# Common datasets specification

## Speech data

- Define top level directory as \<dataset-name\>
- Inside the \<dataset-name\> directory:
	1. Create a file named '\<dataset-name\>\_labels.txt' which contains:
		- \<utt-id\> \<label1\> \<label2\> ... \<labelN\> for each utterance
	2. Create a folder named 'features' which contains:
		- Folders which describe different techniques of extracting features \<feature-type\> (e.g. Hamming_30ms_MFCCs)
	3. Inside each <feature-type> folder:
		- Create a folder for each utterance named \<utt-id\>
		- Inside each \<utt-id\> folder define a file for each frame named '\<utt-id\>\_frame\_\<frame-num\>' that contains the features separated with spaces
