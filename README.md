# PRM Hackathon

## Introduction - Problem 2

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







## Introduction: Problem 4

#### When additional data is provided alongside our files, how is that best displayed to our users? (Design)

We didn't have any user research or access to users during this hackathon, so we took a hypothesis-driven design approach to this problem. This was a combination of:

- using educated guesses on the needs of GPs and medical staff - relying on the knowledge of team members with previous healthcare experience
- UX best practice - where possible, using the components available within the NHS design system and supplementing these with design systems from other government departments

### Tools

- Goodnotes iPad app - to create quick sketches of screens
- Miro - to wireframe screen designs in more detail
- NHS prototype kit - to build a high-fidelity clickable prototype

### Constraints

- We didn't have access to users during the hackathon so we have not validated these designs against hypothetical use cases
- The NHS design system is more limited than other design systems across government, so we needed to re-purpose some components to fit into our design. Creating this prototype in Figma would have allowed us to be less constrained by these limitations but we were hindered by time
- We had to take some 'shortcuts' to quickly build the prototype within the timeframe, so we have gone against best practice in some cases. In a real life scenario, we wouldn't have taken these shortcuts (i.e. deleting the Caption tag as it appeared in the wrong place on the screen)
- We didn't have a content designer on the team, and acknowledge that having someone with content expertise would have improved the quality of the prototype

### Learnings
- A hypothesis-driven design approach is great for quickly building something but we are left with lots of uncertainty about how well this works for users
- More time would have enabled us to implement components from other design systems
- The NHS design system is based around the needs of patients; we aren't sure whether this satisfies the needs of internal staff so more work is needed to better understand this