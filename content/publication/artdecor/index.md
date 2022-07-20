---
title: "Expressing Patient Selection Criteria Based on HL7 V3 Templates Within the Open-Source Tool ART-DECOR"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Christoph Rinner
- Georg Duftschmid

date: "2019-02-09T00:00:00Z"
doi: "https://doi.org/10.1093/bioinformatics/btac068"

# Schedule page publish date (NOT publication's date).
publishDate:

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In Studies in health technology and informatics
publication_short: In Stud Health Technol Inform.

abstract: Background - Reuse of EHR data for selecting patients who are eligible for clinical research can substantially improve the recruitment process. ART-DECOR is an open-source tool that is commonly used to design and publish HL7 V3 templates of national (e.g. ELGA) and international EHR initiatives. Objectives - Extend ART-DECOR to allow the definition of criteria that may be used for patient selection. Methods - Using the native ART-DECOR development framework we extended existing ART-DECOR template associations by allowing conditions to be formulated. Results - An editor for the specification of conditions was implemented. The resulting criteria are internally translated to XPath expressions and can be immediately applied to CDA documents. As a prototypical application of our approach we implemented a "Trial Criteria Evaluator" tool that allows trial eligibility criteria to be composed of our ART-DECOR criteria and have them checked against a patient's CDA documents. Conclusion - Referring to HL7 templates, our criteria can be applied to documents of national EHR systems such as ELGA and hereby reach a broad patient cohort. Implementing our approach within ART-DECOR alleviates its reuse and enhancement by other researchers.



# Summary. An optional shortened abstract.
summary: In this paper, existing ART-DECOR template associations are extended, to supports experts in the formulation of conditions for patient selection in clinical research.

tags: [Electronic Health Records, Patient Selection]

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ebooks.iospress.nl/pdf/doi/10.3233/978-1-61499-971-3-226'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []
  
---
