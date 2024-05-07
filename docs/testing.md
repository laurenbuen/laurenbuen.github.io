# Testing

## Test Plan
These are the manual tests we plan to carry out.

|  Test Case ID | Test Type | Description | Scenario |
| ------------- | ----------- |--------- | ------ |
| TF1.1 | UAT | Requests permission to access user location | <li>1. User clicks "Find Nearest Taxi Rank"</li><li>2. Confirmation box appears, requesting permission.</li> |
| TF1.3 | UAT | Centre map on user location | <li>1. User clicks "Find Nearest Taxi Rank"</li><li>2. User grants permission</li><li>3. Map appears centred on user location </li> |
| TF1.4 | UAT | Add markers for each taxi rank | <li>1. User clicks "Find Nearest Taxi Rank"</li><li>2. User grants permission</li><li>3. Map shows markers for each taxi rank in the area </li>|
| TNF0.1 | UAT | App should work on different browsers e.g. Chrome/Safari etc. |  1. Perform all tests on Chrome / Safari|
| TNF0.4| UAT | Data should be up-to-date; less than one year old | 1. Confirm last update on Bristol Open Data |
| TNF1.1 | UAT | Display up to 10 of the nearest taxi ranks on one page | 1. Confirm that up to 10 taxi ranks can be displayed when user clicks on "Find Nearest Taxi Rank".|
| TNF1.2 | UAT | Default to Bristol City Centre | <li>1. User clicks "Find Nearest Taxi Rank"</li><li>2. User denies permission</li><li>3. Map centred on Bristol City Centre </li> |
| TNF2.1a | UAT | App should take a maximum of 5 seconds to load. | <li>1. User clicks "Find Nearest Taxi Rank"</li><li>2. Map appears within 5 seconds.</li> |
| TNF2.1b | UAT | App should take a maximum of 5 seconds to load. | <li>1. User clicks "Find Taxi by Operating Time"</li><li>2. Table appears within 5 seconds.</li> |


## Requirements Traceability Matrix
The RTM links requirements to code via testing.

| Use-Case ID | Requirement ID | Software module | Test Case | Status |
| ----------- | -------------- | --------- | ------ | ------ |
| UC1 | FR1.1 | index.html | TF1.1 | Pass |
| UC1 | FR1.3 | map.html | TF1.3 | Fail |
| UC1 | FR1.4 | map.html | TF1.4 | Pass |
| UC1 | NFR0.1 | ALL | TNF0.1| Pass |
| UC1 | NFR0.4 | - | TNF0.4| Pass |
| UC1 | NFR1.1 | map.html | TNF1.1 | Pass |
| UC1 | NFR1.2 | map.html | TNF1.2 | Pass |
| UC1 | NFR2.1 | map.html | TNF2.1a | Pass |
| UC1 | NFR2.1 | operating.html | TNF2.1b | Pass |


