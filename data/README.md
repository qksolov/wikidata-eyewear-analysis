# Notable People Dataset (Wikidata-based)

### Dataset Overview

This dataset contains **417,937 biographical records** of notable individuals, extracted from **[Wikidata](https://www.wikidata.org/)** using **SPARQL queries** via the [Wikidata Query Service](https://query.wikidata.org/).  

#### Key Selection Criteria:
- **Timeframe**: Individuals born in the **20th or 21st century** (1901–present).  
- **Country of Birth**: Entries must include the `country_of_birth`.  
- **Photo Availability**: Each entry includes an associated image (`image_url` is mandatory).  
- **Profession Filter**: Focused on individuals with occupations categorized in `occupation_groups.csv` (_Science & Academia_, _Arts & Culture_, _Public Figures_, _Sports_, _Business_).  

---

### Column Descriptions  

| Column                      | Description                                                                 | Notes                          |  
|-----------------------------|-----------------------------------------------------------------------------|--------------------------------|  
| `wikidata_url`              | Unique Wikidata URL identifier for the entry                              | Mandatory                      |  
| `label`                     | Primary name/label of the person (usually in English)                     | Mandatory                      |  
| `name_in_native_languages`  | Name(s) in the person’s native language(s)                                 | `;`-separated values           |  
| `pseudonyms`                | Alternative names or aliases used by the person                            | `;`-separated values           |  
| `sex_or_gender`             | Gender information                                                         | Mandatory                      |  
| `date_of_birth`             | Birth date                                                                 | Mandatory                      |  
| `place_of_birth`            | City or region of birth                                                    |                                |  
| `country_of_birth`          | Country of birth                                                           | Mandatory                      |  
| `date_of_death`             | Death date (if applicable)                                                 |                                |  
| `place_of_death`            | City or region of death (if applicable)                                    |                                |  
| `country_of_death`          | Country of death (if applicable)                                           |                                |  
| `citizenships`              | Nationalities or citizenships held                                         | `;`-separated values           |  
| `occupations`               | Specific occupations or roles                                              | Mandatory, `;`-separated       |  
| `occupation_groups`         | Broad occupational categories                                              | Mandatory, `;`-separated       |  
| `awards`                    | Awards, honors, or recognitions received                                   | `;`-separated values           |  
| `signature_url`             | URL to an image of the person’s signature                                  |                                |  
| `image_url`                 | URL to the person's image/portrait                                         | Mandatory                      |  
| `date_of_image`             | Date when the image was created (if available)                             |                                |  

---

### Notes

The data may contain some number of inaccuracies, due to inconsistencies or errors in the original Wikidata entries. This can sometimes be seen in date fields, especially `date_of_image`.


### Source and Licensing Notes

- All data in this dataset was derived from **[Wikidata](https://www.wikidata.org/)**. Wikidata content is available under the [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
- Images linked in `image_url` and `signature_url` are hosted on **[Wikimedia Commons](https://commons.wikimedia.org/)** and may have individual licenses (e.g., CC BY-SA, Public Domain). Please check the license terms on the source page before using.
