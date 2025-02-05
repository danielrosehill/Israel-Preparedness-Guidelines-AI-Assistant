# Israel Preparedness Guidelines - AI Assistant

This repository contains contextual data and a system prompt for an AI assistant tasked with providing users with datestamped emergency guidelines from Israel's civilian preparedness body, the Home Front Command (Hebrew: Pikud HaOref).

#git# Repository Structure

The repository is organized into the following main directories:

### `/context-data`
Contains the emergency guidelines and reference data organized by language and date:
- `/en` - English language data
  - `/06_feb_2025` - Date-stamped content from Home Front Command
    - `/home-front-command-import` - Official guidelines for various emergency scenarios
      - `/earthquakes` - Earthquake preparation and response guidelines
      - `/general` - General emergency preparedness information
      - `/hazmats` - Hazardous materials guidelines
      - `/home-safety` - Home safety and fire prevention
      - `/hostile-aerial-vehicles` - Guidelines for aerial threats
    - `/public-shelter-lists` - CSV files containing public shelter locations
  - `/other-data` - Additional reference information
    - Emergency phone numbers
    - Official HFC URLs
    - Red Alert application information

### `/system-prompts`
Contains the prompt templates used to configure the AI assistant:
- `english-rag.md` - System prompt for the English language assistant

## Setup Instructions

To create an AI assistant using this repository:

1. **Choose an Implementation Model:**
   - Static Data: Use the provided date-stamped data
   - Live Data: Configure with direct URL access (implementation details not included)
   - Hybrid Model: Use periodic data ingestion from trusted sources

2. **Configure the Assistant:**
   - Use the system prompt from `/system-prompts/english-rag.md`
   - Load the contextual data from `/context-data`
   - Ensure the assistant acknowledges:
     - It is not an official government resource
     - The date of its last data update
     - Its limitations and the need to refer to official sources

3. **Provide Context Data:**
   - Emergency guidelines from the Home Front Command
   - Lists of official URLs
   - Emergency phone numbers
   - Public shelter locations
   - Red Alert app information

## Implementation Options

### Implementation 1 - Live Data
A version that could be configured with direct URL access and a whitelist of reference URLs.

### Implementation 2 - Static Data
Uses periodic timestamped imports from trusted resources provided as contextual data to the Assistant.

### Implementation 3 - Hybrid Model
Utilizes a scraping script to periodically ingest updated guidelines from trusted resources, potentially using APIs like Firecrawl for ingesting contextual data from unstructured web resources.

## Author

Daniel Rosehill  
(public at danielrosehill dot com)

## Licensing

This repository is licensed under CC-BY-4.0 (Attribution 4.0 International) 
[License](https://creativecommons.org/licenses/by/4.0/)

### Summary of the License
The Creative Commons Attribution 4.0 International (CC BY 4.0) license allows others to:
- **Share**: Copy and redistribute the material in any medium or format.
- **Adapt**: Remix, transform, and build upon the material for any purpose, even commercially.

The licensor cannot revoke these freedoms as long as you follow the license terms.

#### License Terms
- **Attribution**: You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
- **No additional restrictions**: You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

For the full legal code, please visit the [Creative Commons website](https://creativecommons.org/licenses/by/4.0/legalcode).
