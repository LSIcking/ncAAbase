# iNClusive Updates

## Update Summer 2024 (starting 15.05.2024)

The update was started by scraping new papers for the paperbase with the keywords listed in the paper ("Mass spectrometry" "tRNA synthetase" "unnatural amino acid", ...). The search was conducted for papers published in 2023-2024, no further time specification could be achieved as ‘Publish Or Perish 8’ does not have this function.
New Papers were scraped on 15.05.2024 with the following amounts

| MS termology              | UAA  | ncAA | nsAA |
| ------------------------- | ---: | ---: | ---: |
| ‘Mass spectrometry’       |  194 |  149 |    8 |
| ‘Electrospray ionization’ |   39 |   31 |    3 |
| ‘Electrospray ionisation’ |    3 |    4 |    1 |
| ‘MALDI’                   |   41 |   44 |    2 |
| ‘MS/MS’                   |   79 |   62 |    6 |
| ‘LC MS’                   |  105 |   75 |    5 |
| ‘GC MS’                   |    6 |    4 |    1 |
| ‘HPLC MS’                 |    6 |    5 |    1 |

## Removing duplications and sorting research articles

After merging the various scraped entries, duplicates were removed using Excel's "Remove duplicates" function. The publications were checked for duplicates via the "Title" header by comparing them with the title of the publication. After removing the duplicates (571 duplicates between hits), 321 remained for further analysis. Before further processing, these hits were compared with the entries from the first publication that had already been processed. After deducting the hits that had already been processed, 138 hits remained. These hits were then manually checked for dissertations (brown), reviews and books (purple), preprints (blue), protocols (orange), English-language research articles (green), and research articles in a language other than English (yellow). As only English-language primary research articles were processed, 64 articles remained. In addition, 4 research articles were not included as they did not meet the criteria of these articles, as well as 14 research articles that were stuck in our pipeline. Between the 4 and 14 research articles, 1 duplicate was found. This leaves 81 peer-reviewed research articles to be processed for the 2024 summer update.

## Analysing each research paper
Please try to work the online version so we don't process articles multiple times
The papers that have to be processed can now be found in "Paperbase summer 2024.xlsx" inside of the "Database Update Summer 2024" folder. The entries should be entered in the "raw data update summer 2024.xlsx" file. The construction of entries is very similar to the previous version with a minor change. **Now, only the link to the PubChem site of the ncAA has to be supplied, the IUPAC, chemical formula, as well as the IUPAC name, will now be added via a script**. Please work through the entries from the top to the bottom as some entries might depend on previous entries regarding further information. Filtering-wise, one of the specific Mass spec terms, tRNA synthetase as well as one descriptive term for ncAA should already be available, therefore no further filtering is necessary. Sometimes the authors used auxotrophic strains were an endogenous tRNA/synthetase pair was used to incorporate the ncAA (no engineered tRNA/tRNA-Synthetase-pair is used). These papers can be discarded but please note it in the paperbase.

Now, onto entering information into the raw database.
### **ID**: 
ID of the entry. Nothing to change here. If we run out of entries, just create new ones. 

### **amino acid abbreviation**: 
Insert the amino acid abbreviation used in the paper here. If there’s no abbreviation mentioned, put **not available** (exactly how it is written here, this will make further processing much easier).

### **amino acid name in the paper**: 
Insert the name of the ncAA used in the paper here. If multiple names occur, please use the most abundant name in the paper

### **amino acid IUPAC**: 
*automated by script*

### **Chemical formula**: 
*automated by script*

### **SMILES**: 
*automated by script*

###**Derivative**: 
If you can make out the canonical amino acid the ncAA is similar to, add it to this column 

### **Function**: 
If a function is mentioned in the paper (e.g., photo-crosslinking) please add the function to this column. Try to use the same terms, as already used in the database (this makes it easier for scientists to search for use cases)

### **aaRS origin organism + amino acid**: 
Insert the original aaRS name here. First term the organism, where the RS natively occurs plus the amino acid that would have been naturally loaded, plus ‘RS’ (e.g., **Mj-TyrRS** – Methanocaldococcus jannaschii Tyrosine tRNA synthetase).  

### **aaRS Mutations**: 
Insert the mutations that have been incorporated into the synthetase here (e.g., **Y32T, E107N, D158P, I159L, L162Q, D286R**). 

### **aaRS organism Name**: 
Insert the name of the organism the aaRS originates from (e.g., **Methanocaldococcus jannaschii**)

### **tRNA name**: 
Check, if this tRNA was previously used and was already inserted into the database. Please insert the tRNA as follows - e.g. **Mj-tRNA Cys CUA** - Mj for the organism (Methanocaldococcus jannaschii), Cys for the amino acid that would be naturally loaded onto this tRNA and CUA regarding the codon that was used. Many documented use cases with their respective sequence will be listed in this document [WIP]

### **tRNA organism**: 
Insert the name of the organism the tRNA originates from (e.g., **Methanocaldococcus jannaschii**) 

### **tRNA seq**: 
Insert the name of the tRNA sequence if available. If too hard to find, please leave it empty and we will find the sequence. 

### **Codon suppression**: 
Please put the **ANTI-CODON** (very important) used in the paper, from there, we will insert the incorporation technique

### **tested in which protein**: 
Please insert the protein name (e.g. **sfGFP**) as written in the paper

### **position in tested Protein**: 
Check for the position that was mutated to another codon for the introduction of the ncAA. Write it as amino acid that got changed + position; if more the one AA is exchanged at the same time in the protein, set a ‘+’ between the positions (e.g. G234+F278); if different positions were tested put a semicolon ‘;’ in between (e.g. G122; A123; D124). Also combinations possible (e.g. G122; A123; D124; F278; G122+F278; A123+D124). If only the position and not the amino acid is give add ‘(aa. not specified)’ (e.g. 122 (aa. not specified)). 

### **test in which Organism**: 
check the paper in which organism + strain they have tested the system. If multiple organisms were used, make a second entry where you just exchange the organism (e.g. Escherichia coli BL21-Gold(DE3))

### **publication**: 
for the publication, just plug the name of the paper into google scholar, click on cite and copy the APA style citation.

### **DOI**: 
Copy the DOI-link directly from the journal cite. Please make sure you are not just copying the Doi (10/11010...) but the whole link starting with “https:” 

### **Link to Pubchem**: 
If you can find a link (e.g **. https://pubchem.ncbi.nlm.nih.gov/compound/3080772**) for the ncAA for PubChem, please put it here. *Very necessary for the script!*

### **Person responsible for the entry**: 
Please insert your name



## Further ressources
PubChem                                - https://pubchem.ncbi.nlm.nih.gov/

Google Scholar                         - https://scholar.google.com/

Optical Structure Recognition A (OSRA) - https://cactus.nci.nih.gov/cgi-bin/osra/index.cgi


