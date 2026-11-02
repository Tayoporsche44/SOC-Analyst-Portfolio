# The Planet's Prestige - Phishing Investigation

## Case Overview
- **Investigation Type:** Phishing / Suspicious Email Analysis
- **Analyst:** Tayo Francis
- **Environment:** Isolated SOC Lab - Ubuntu
- **Status:** Completed

## Executive Summary
Investigated a suspicious email titled *A Hope to CoCanDa*. Header analysis revealed sender spoofing, SPF failure, and a suspicious Reply-To address. The attachment was disguised as a PDF but identified as a ZIP archive through magic-byte analysis. Extracted files and supporting documents were examined to identify attacker information and a suspected command-and-control domain.

## Key Findings
| Finding | Result |
|---|---|
| Displayed Sender | Bill |
| Sender Address | billjobs@microapple.com |
| Email Service | emkei.cz |
| SPF | Fail |
| Reply-To | negeja3921@pashter.com |
| Actual Attachment Type | ZIP |
| Malicious Actor | Pestero Negeja |
| Attacker Location | The Martian Colony, Beside Interplanetary Spaceport |
| Probable C2 Domain | pashter.com |

## Investigation Report
[View the Full Investigation Report (PDF)](./The-Planets-Prestige-Investigation-Report.pdf)

## Investigation Evidence
Screenshots documenting the investigation process:

[View Investigation Screenshots](./Screenshots/)

## Investigation Methodology
1. Email header and sender authentication analysis.
2. MIME structure and attachment filename analysis.
3. File magic-byte identification.
4. ZIP archive extraction and evidence verification.
5. PDF metadata and message analysis.
6. Excel workbook investigation.
7. Base64 decoding and attacker location identification.
8. IOC identification and defensive recommendations.

## Conclusion
The investigation identified a phishing email containing a disguised ZIP attachment and attacker-related indicators. The findings support treating the message and its attachment as malicious.
