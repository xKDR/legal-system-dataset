# Legal System Dataset

This repository contains datasets and an analysis notebook for exploring case data from Indian courts.

## Structure
- `data/` – zip folders for datasets on Bombay High Court and National Company Law Tribunal - Mumbai bench cases 
- `analysis.ipynb` – Jupyter notebook with exploratory analysis

### Bombay High Court
#### Variables 

| Name | Format | Description |
|------|--------|-------------|
| `filing_no` | string | Case filing number as given by the Bombay High Court|
| `court_name` | string | Name of the court where the case was filed |
| `cnr` | string| Case number recorded, a unique 16-digit number assigned by e-Courts |
| `filing_date` | yyyy-mm-dd | Date the case was filed |
| `disposal_date` | yyyy-mm-dd  | Date the case was disposed |
| `hearing_date` | yyyy-mm-dd | Date of the hearing |
| `case_status` | Categorical | Current status of the case (e.g., Pending, Disposed) |
| `case_typology` | Categorical | Type of case (e.g., Original_Commercial Suit, Original_SUITS) as given by the Bombay High Court|
| `case_category` | Categorical | XKDR-generated groupings of similar typologies (e.g., Suits, Commercial) |
| `case_nature` | Binary |  Identifies whether a matter is the primarily instituted case or a case connected to it - Main/Connected |
| `main_matter_filing_no` | string | Case filing number of the primarily instituted case as given by the Bombay High Court |
| `updated_on` | yyyy-mm-dd | The date of last update of the particular matter by XKDR |


### National Company Law Tribunal
#### Variables 

| Name | Format | Description |
|------|--------|-------------|
| `filing_no` | Number | Case filing number |
| `court_name` | Text | Name of the court where the case was filed |
| `filing_date` | yyyy-mm-dd | Date the case was filed |
| `disposal_date` | yyyy-mm-dd | Date the case was disposed |
| `hearing_date` | yyyy-mm-dd | Date of the hearing |
| `case_status` | Text | Current status of the case (e.g., Pending, Disposed) |
| `case_typology` | Text | Type of case (Insolvency) |
| `registration_number` | Text | Registration number assigned to the case by the court |
| `case_nature` | Binary |  Identifies whether a matter is the primarily instituted case or a case connected to it - Main/Connected |
| `case_category` | Categorical | XKDR-generated groupings of similar typologies (e.g: IBC) |
| `main_matter_filing_no` | string | Case filing number of the primarly instituted case as given by the National Company Law Tribunal | 
| `updated_on` | yyyy-mm-dd | The date of last update of the particular matter |


## Citation

If using this dataset, please cite as:

> XKDR Forum (2025). *Legal System Dataset*. [https://xkdr.org](https://xkdr.org)

## Note

We believe the data to be comprehensive to the extent the courts have made the data publicly available and searchable on their website. 