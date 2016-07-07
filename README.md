# test
CODE FILES:
ProductAspectExtraction.java : Main files containing the rules.
DependencyParserImp.java : Support files to apply Dependency Parsing


PATH DEPENDENCIES: Set the following paths correctly.
Line 34: Parser Model path is set.
Line 37: DependencyParserImp class object created.
Line 45: INPUT:  Initial opinion words are read from the file “positive.txt”. Set the path correctly.
Line 54: INPUT: Initial opinion words are read from the file “negative.txt”. Set the path correctly.
Line 73: INPUT: Set the path for correctly formatted review data file. I have used “sample3.txt” for the same purpose.
Line 124: Set the path correctly for MaxEnt Tagger.
Line 937: OUTPUT: Initial Features Set are obtained.Set the output correctly.
Line 963: INPUT: Set the path for correctly formatted review data file. I have used “sample3.txt” for the same purpose.
Line 1010: Set the path correctly for  MaxEnt tagger
Line 1099: OUTPUT: Freq_Feature file is obtained which gives our features Set along with their frequency.
Line 1124 : Opinion Set is obtained and printed in this line.
Line 1159: Threshold for filtering Features is set. Here, I have set threshold as 0.For Larger Datasets e need to set an appropriate Threshold.
Line 1170:  FinalFeature Set is printed in this line.Set the o/p path correctly.
Line 1200: FINAL OUTPUT : The Final Annoted File is obtained here. Set the path correctly. 

INPUT FORMAT
INPUT REVIEW DATA: (Sample)
B0009B0IX4,5.0,Works well, good audio quality, battery lasts a long time.
The first part denotes the Product ID followed by the review rating score. The last part contains the review text followed by a new line character. Each part is comma separated.
OUTPUT FORMAT : (Sample)
21@headsets@1
The first part denotes the review ID followed by the Product aspect word which is again followed by Opinion Polarity.
Each part are ‘@’ separated.

INPUT FILES REQUIRED:
1) sample3.txt: Demo Review Data
2) positive.txt: Initial Positive Opinion Words
3) negative.txt: Initial Negative Opinion Words
OUTPUT FILES GENERATED:
1) initialFeatures.txt :Initial Features Set
2) Freq_Feature.txt : Features Set along with their frequencies
3) opine3.txt : Final Expanded Opinion Set
4) FinalFeature.txt : Final Filtered Features Set based on the user Set threshold.
5) annote.txt : Final OUTPUT FILE

JAR FILES REQUIRED
1) english_SD.gz
2) english_UD.gz
3) englishPCFG.ser.gz
4) english-bidirectional-distsim.tagger
5) english-bidirectional-distsim.tagger.props

All the jar files are publicly available in http://nlp.stanford.edu/software/lex-parser.shtml#Download .
