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
The papers that have to be processed can now be found in "Paperbase summer 2024.xlsx" inside of the "Database Update Summer 2024" folder. The entries should be entered in the "raw data update summer 2024.xlsx" file. The construction of entries is very similar to the previous version with a minor change. **Now, only the link to the PubChem site of the ncAA has to be supplied, the IUPAC, chemical formula, as well as the IUPAC name, will now be added via a script**. Please work through the entries from the top to the bottom as some entries might depend on previous entries regarding further information. Filtering-wise, one of the specific Mass spec terms, tRNA synthetase as well as one descriptive term for ncAA should already be available, therefore no further filtering is necessary.



## Further ressources
PubChem                                - https://pubchem.ncbi.nlm.nih.gov/

Google Scholar                         - https://scholar.google.com/

Optical Structure Recognition A (OSRA) - https://cactus.nci.nih.gov/cgi-bin/osra/index.cgi


