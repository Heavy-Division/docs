# Heavy Division Quality Assurance Team 
Thank you for participating in QA for the B78XH project. Your role will be crucial in ensuring the 
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
reports at least twice a month. In certain cases such as lulls in the development cycle or a personal circumstance,
this requirement will be waived. Please reach out to an admin if you need to take leave from the QA team.

## Reports 
To fill out a report, simply copy and paste the [template]() onto a comment in a developer Pull Request in the B78XH repository: 

Every developer Pull Request will include instructions for testing. Contact the author of the PR if you need additional information.

## Workflow 
As mentioned above, you will either be testing mass reported features or pre-release builds. 
The former will be carried out under the Issues tab in github whilst the latter will take place in the Pull Request github.<br>

### Ready for Review
When a developer is ready to have their PR reviewed, they will mark it as ready for review by changing it from a draft to a formal pull request.
Each feature or change will require different testing methods, so it is important you read the developer's instructions for testing.<br>

### Code Check
Once a pull request is ready for review, it will require a code-check first, meaning that the change is up to the Heavy Division programming [standards]() and there are no glaring errors present. When signing up for the QA role please 
indicate if you are able and willing to perform code checks.<br>

### QA Review
Once the code-check is completed the QA team will need to test the build in-sim.<br>

After review, the QA team can sign off on the build as finished, request action from the PR author, or cancel the review if the author cancels the PR.<br>

## Overview
The stages of testing should look like:<br>
Ready for Review -> Code Check -> QA Team Review & Report -> Action from author / Finalization / cancellation. 
