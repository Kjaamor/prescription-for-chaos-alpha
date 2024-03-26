## PRM Hackathon

### Introduction - Problem 2

#### How effective is Optical Character Recognition on free-hand writing with GP notes (messy) in mind? (AWS)

In addition to its electronic records system, many important medical documents exist as Lloyd-George records; records kept on paper file. These records can contain information that is critical to GP practioners in understanding their patients' health needs. A system that enables us to extract text and numeric data from written notes so that this can be processed in conjunction with the online system would improve patient care.

AWS Textract is a tool that could be used in this regard. We should review the accuracy of this tool when used against notes and handwriting to judge its potential benefits, risks and create a plan for implementation.

### Toolings

- Main system under test: AWS Textract
- S3 bucket for storage of files
- Files uploaded through API
- AWS Lambda function runs Textract

### Method of Assessment

We collected many different sample images of handwriting from a Google image search. These items were selected based on their resemblence to medical notes. Notes were broadly grouped into 5 tiers of readability, with the most human-legible notes in tier 1, and the most human-illegible in tier five.

Each piece was passed through the Textract Lambda, extracting the parsed text and the lambda's confidence level in its assessment. For each piece a team member would write their own human parsing of the image text, and provide their own assessment of their "human confidence level" in their parsing. The team member would then compare the human reading and Textract readings and evaluate Textract on how close it was to the human reading.

### Findings

TBC

See table:

### Themes

TBC

- How did Textract perform in each group? Was it better than others?
- How did Textract's confidence mirror human confidence? Where is the cut-off?
- Were there any other themes identified from this

### Other Randoms Thoughts

- AI when extracting from our first image ("Betterhandwriting.png") AI identified the word "woodm". This wouldn't be identified
by other AI toolings, or even spellcheck.

- AI sometimes has level of confidence in reading messy handwriting that falsely high, when compared to human reading

### Conclusions

TBC

General assessment on usefulness, risks, potential cut offs, and mitigations.

### Limitations/Further research required

- Greater sets of data for Textract to be assessed on
- Greater variety (and experience - medical clerks!) in humans reviewing test text
- Suitable blinding
- 







### - Introduction: Problem 4

#### When additional data is provided alongside our files, how is that best displayed to our users? (Design)

*James to write content to follow based on Dani's presentation*