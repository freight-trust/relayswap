# Continuous Oversight & Protocol DevOps


- [Continuous Oversight & Protocol DevOps](#continuous-oversight---protocol-devops)
  * [Solidity Conventions](#solidity-conventions)
  * [Security](#security)
  * [Smart Contract Disclaimer & DevOps](#smart-contract-disclaimer---devops)
      - [Fail Safe Mechanism](#fail-safe-mechanism)
      - [Monitoring](#monitoring)
        * [Active Monitoring](#active-monitoring)



> Note: Read our IRP, Defects, and other Disclaimers here: [Freight Trust Omnibus Documentation](https://ft-docs.netlify.app/operations/irp/)


## Solidity Conventions 


We use leading underscores and mark `struct`s to make it clear to the user that its contents and layout are not part of the API.

pragma => 0.4.22> <=5.90 

Ideally = 0.5.11=>  <=0.7.0

## Security 

See [Security](./.github/SECURITY.md)

support@freight.zendesk.com 

Please Read our SOFTWARE DEFECTS, INCIDENT RESPONSE PLAN, and [SMART CONTRACT PRACTICES](https://ft-docs.netlify.app/blockchain/smart-contract-dev/) 

## Smart Contract Disclaimer & DevOps

#### Fail Safe Mechanism

Smart contracts may not include appropriate or sufficient backup / failover mechanisms in case something goes awry.

Smart contracts may depend on other systems to fulfill contract terms. These other systems may have vulnerabilities that could prevent the smart contract from functioning as intended.

Some smart contract platforms may be missing critical system safeguards and customer protections.

Where smart contracts are linked to a blockchain, forks in the chain could create operational problems.

In case of an operational failure, recourse may be limited or non-existent — complete loss of a virtual asset is possible.

Please read our [DISCLAIMERS](./DISCLAIMERS.md) && [SOFTWARE DEFECTS](./SOFTWARE_DEFECTS.md)


#### Monitoring 

** We monitor **

* Governance. 
Smart contracts may require attention, action, and possible revision subject to appropriate governance and liability mechanisms.

* Application State
Low Level Monotiroing of Deployed Contracts

* Suspicous Activity
Failsafe mechanism to return to us in case of attack or error


##### Active Monitoring

Smart Contract Monitoring:
Actively monitor one (or more) Ethereum smart contracts and user accounts (or any combination) watching for odd or “known-dangerous” transactional patterns. Report to anomalies to a list of email, SMS, web site, or individuals whenever something of interest happens.
End Users:	Smart contract developers, smart contract participants (i.e. token holders)
Notes:	“Weird” things include recursive attacks, violations of invariants (token balances to ether balance), largest purchases, most active trader accounts, etc.; Could potentially spawn an “insured” smart contract industry expectation.
Smart Contract Reporting:

“Quarterly” reports may be available. On demand reports generated for margin accounts, activity (report on token holders), individual ether holdings and transaction histories (i.e. bank statements) on a per-account, per-contract-group, by industry, or system wide.
End Users:	Smart contract developers, smart contract participants (i.e. token holders), economists, regulators. 

Please see our [DOCUMENT RETENTION POLICY](./DOCUMENT_RETENTION_POLICY.md)

*NOTE*:	Allows for self-reporting on business processes, expenditures, and revenue from outside an organization—​no need to wait for company reports; marketing efforts might engender an expectation that every smart contract’s accounting is fully transparent.
Auditing Support:

Provide data and transactional information to third parties not associated with the development team of a smart contract system. Interesting to potential investors, industry analysts, auditors and/or regulators.

End Users:	regulators, auditors, potential investors
*NOTE*:	Fully parsed data makes for much easier auditing of smart contracts, could expose non-delivery of promised behavior.