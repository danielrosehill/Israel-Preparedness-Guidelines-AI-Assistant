# Israel Preparedness Guidelines - AI Assistant

This repository contains contextual data and a system prompt for an AI assistant tasked with providing users with datestampped emergency guidelines from Israel's civilian preparedness body, the Home Front Command (Hebrew: Pikud HaOref).

## Implementation 1 - Live Data

Not modeled in this repository is a version of this Assistant that could be configured with a live data tool (direct URL access and whitelist of reference URLs.)

## Implementation 2 - Static Data

The static version of this configuration uses a periodic timestamped import from a trusted resource and provides that as contextual data to the Assistant. 

## Implementation 3 - Hybrid Model

A third model, also not shown in this configuration, would be utilizing a scraping script in order to periodically ingest updated guidelines from a trusted resource.  This could be achieved quite easily using one of the Apis for providing LLMs with contextual data from unstructured web resources (Firecrawl etc).

In this implementation, a white list of trusted URLs could again be used for the purpose of grounding. 

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