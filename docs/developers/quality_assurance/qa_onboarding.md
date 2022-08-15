# Heavy Division Quality Assurance Team 
As a Quality Assurance Tester, your role will be crucial in ensuring the 
stability and performance of the aircraft over the life of the simulator. 

The QA role has two main responsibilities: 
1. Testing user-reported errors 
2. Testing pre-release builds 

If a significant number of users report a bug associated with the aircraft, it is up to the QA team 
to reproduce the issue and document it as thoroughly as possible so our developers can focus on fixing it. 

## Testing Setups
As a tester you will have at minimum the following specs:<br>

|                | AMD           | NVIDIA         |
|----------------|---------------|----------------|
| MIN OS Version | Windows 10    | Windows 10     |
| CPU            | Ryzen 5 1500X | Intel i5-8400  |
| GPU            | Radeon RX 590 | NVIDIA GTX 970 |
| VRAM           | 4 GB          | 4 GB           |
| RAM            | 16 GB         | 16 GB          |
| HDD            | 150 GB        | 150 GB         |
| Bandwidth      | 20 Mbps       | 20 Mbps        |
> Source: [FAQ: Recommended MSFS specs](https://flightsimulator.zendesk.com/hc/en-us/articles/360013463459-Minimum-Recommended-and-Ideal-PC-Specifications-for-Microsoft-Flight-Simulator)

Please ensure your system meets these requirements before applying to the QA program. 

## Maintaining QA role 
In order to maintain your role on the QA team you will be required to conduct tests and submit 
reports on a regular basis. In certain cases such as lulls in the development cycle or a personal circumstances,
this requirement will be waived. Please reach out to an admin if you need to take leave from the QA team.

## Reports 
To fill out a report, simply copy and paste the [template](#template) onto a comment in a developer Pull Request in the B78XH repository. Every developer Pull Request will include instructions for testing. Contact the author of the PR if you need additional information.

## Workflow 
As mentioned above, testing involves either mass reported features or pre-release builds. The former is carried out under the Issues tab in github whilst the latter takes place in the Pull Request github.

### Ready for Review
When a developer is ready to have their PR reviewed, they will mark it as ready for review by changing it from a draft to a formal pull request.
Each feature or change will require different testing methods, so it is important you read the developer's instructions for testing.

### Code Check
Once a pull request is ready for review, it will require a code-check first, meaning that the PR follows styling and formatting guidelines and there are no glaring errors present. When signing up for the QA role please 
indicate if you are able and willing to perform code checks.

### QA Review
Once the code-check is completed the QA team can test the build in-sim.

To do this, head to the Open Pull Request and navigate to the requester's forked repository. Download the zip file and extract to your community folder (if you already have B78XH installed, move it to a separate location such as the desktop to avoid conflicts). Be sure to read the instructions written on the PR for testers.

#### QA Tiers for PRs

The Heavy Division developers are required to categorize their PRs into two test tiers to indicate the complexity or importance of the PR.

More complex features or features vital for the stability of the add-on will need considerably more testing than a simple change of a button text.

The developer, developer leader and QA leader determine the tier of testing required and how many successful tests must be reported before a PR can be accepted and merged into the master branch.
Tier 1

    Extensive and careful testing is expected but no full flight is required.
    Providing media is not required.
    Of course you can always do a full flight and provide media but the test is valid without it.

Tier 2

    At least one full flight is required to test Tier 2.
    Providing media (screenshots/videos) is a requirement especially for any issues that might arise.
    Tests without a full flight or media are not valid and will require another tester to still do a full tier 2 test
After review, the QA team can sign off on the build as finished, request action from the PR author, or cancel the review if the author cancels the PR.

## Overview
The stages of testing should look like:
Ready for Review -> Code Check -> QA Team Review & Report -> Action from author / Finalization / cancellation. 

![image](/docs/assets/qa_workflow.png)

# Template 
```md
Quality Assurance Tester/Trainee Report

Discord          : (name#1234)
Object of testing: (#PR Number)
Tier of Testing  : (1/2)
Date             : (DD/MM/YYYY)

Testing Process: 
(Detail is needed)

Negatives:       
(Any issues, doubts. - type N/A if none are found)

Testing Results: 
(Passed/Not Passed)

Conclusions: 
(Notes made, the positives in the PR, and anything extra you would like 
to mention - Delete Line if Nothing Extra is to be mentioned)

Media:       
(Pictures/videos if applicable - delete line if not applicable)
```