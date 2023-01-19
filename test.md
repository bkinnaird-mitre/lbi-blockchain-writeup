# Blockchain Use Cases Decision Tree

## Objective

This document will provide a high level workflow that can be used to identify scenarios where blockchain technologies may be advantageous.  Using this workflow, in combination with IRS subject matter experts, specific use cases where blockchain may be applicable are identified for further exploration. 

## Executive Summary

This document serves as a guide for determining the applicability of blockchain based on a short list of attributes associated with the use case in question.  In general, use of blockchain technology can be summarized as:
- most approprate for distributed, low-trust environments
- not ideal for storing large amounts of non-transactional data
- not appropriate for mutable data, or in single-entity environments
- significantly more difficult to provision and maintain than traditional databases

## What is Blockchain?

A ‘blockchain’ is a distributed digital ledger that is used to record transactions.  It is an immutable database, which means that information cannot be tampered with or altered once it has been recorded.  If there is an error in an entry, then a new, revised entry must be made, and both entries will subsequently be visible on the ledger.

The name comes from the fact that a blockchain stores data in blocks, individual units that are linked, or ‘chained’, together.  New data is filed into blocks – and blocks are subsequently chained together – in chronological order, so a blockchain becomes longer and longer as more information is added to it.  

Each new piece of information is also assigned a timestamp, which makes it easy for users to find out exactly when it was added to the chain.  The transparency and immutability of the blockchain makes it a very reliable and trustworthy business resource both for individuals and companies.

![Figure 1: Blockchain transaction flow](images/image_20230105171112.png)
*Figure 1: Blockchain transaction flow*

In the context of blockchain, a decentralized system is one that is controlled in equal measure by each of its constituent parts.  No single individual, corporation or other entity can exert a disproportionate degree of control over how they are constructed and run. In contrast, a centralized system is controlled and organized according to a rigid hierarchical structure.  In such a system, power and decision-making authority is concentrated in the hands of a relatively small number of individuals at the top of the hierarchy. 

To fit the blockchain technology into modern, security-oriented contexts, two primary blockchain models have evolved: permissioned and permissionless.  In the permissionless model, which is also known as a public blockchain, there are no restrictions and participation is not controlled by an administrator.  In a permissioned blockchain, the distributed ledger can only be accessed by people who are allowed to do so by the administrator. These users are provided different types of privileges which allows them to do certain actions. While most of the public coverage of blockchain technology is centered on a pure permissionless and public blockchain network solution  most business solutions will contain a hybrid of characteristics of public/private and permissioned/permissionless implementations.  

## When to Use Blockchain

Blockchain provides a unique ledger that provides a high degree of transparency, data reliability, and security. It has been used in both financial and non-financial contexts. Among a wealth of potential uses, it has been used to facilitate the tracking of supply chains, verify records and digital identities, and in the automatic disbursement of funds such as grants. 

Blockchain was designed to provide transparency in transactions making it well suited for low-trust scenarios. The cryptographically secure ledger makes it suitable when a historical record of data is required over just the final value. Blockchain also works well in situations where there is an intermediary such as a broker that can be eliminated to increase efficiency. Finally, blockchain naturally finds success when managing native digital assets.

As mentioned earlier, blockchain works well in low trust environments such as when there are multiple organizations involved and does not require a central authority. It allows all stakeholders to take advantage of the transparency and security of the chain to verify transactions. In addition, the shared ledger and write access for all nodes can increase data sharing potential within a set of organizations. 

Due to its inherent immutability, blockchain is a good fit when an application requires a strongly auditable, tamperproof ledger of transactions. As such, it is especially suited for cases involving the creation and transfer of assets. Transactions on the chain are highly visible and can be effectively traced to their source. 

Additionally, blockchain provides data reliability due to its decentralized nature, by providing redundant copies of the data and removing any centralized point of failure. Decentralization, when combined with the cryptographic chaining, effectively prevents tampering and allows blockchain to provide a great degree of traceability and ownership verification.

## Blockchain Challenges

Blockchain is not a perfect fit for every application – potential use cases should be considered carefully against a more traditional database or hybrid solution. For example, if there is only one entity, a blockchain system could be redundant. Unlike a traditional database, the immutability of a blockchain means that while all changes can be tracked, there is no way to update, remove, or edit records after they are added. This also means that care should be taken with data privacy concerns before choosing blockchain as data cannot be removed.  

Blockchain also has several structural considerations. It is not a good fit for storing large amounts of non-transactional data. It can also have issues with scalability as the nodes required can be expensive and computationally heavy. The verification process for transactions can be slow in certain blockchain systems which may present a scaling issue with applications that intend to handle a high number of transactions per second.

![[Pasted image 20230105170926.png]] 
*Figure 2: Blockchain Usage Decision Tree*
  
## Conclusion

Although blockchain is not always the best fit for all applications, it does have numerous benefits that make it a suitable technology when used correctly.  The blockchain technology and its use cases will continue to expand, mature, and evolve. In parallel the decision tree should continue to expand, mature, and evolve to keep assisting the IRS in identifying the applications that could benefit from using blockchain.

# Appendix A: TradeLens and the International Supply Chain

TradeLens was a blockchain based trade platform developed by IBM in conjunction with Maersk, a container shipping company. TradeLens attempted to provide transparency to the complex international trade system. Processing documents related to container shipping often costs more than the transportation, and the physical movement of paperwork is prone to delays, extra costs, and is prone to inconsistencies that cannot be traced easily. Efficient management and addressing inconsistencies is vital as this paperwork is used to address counterfeiting, smuggling, and even trafficking. 

TradeLens facilitated document workflow by allowing stakeholders to access and digitally sign documents in real time while taking advantage of the unique properties of the blockchain primarily for its powerful historical ledger providing accessibility and security in a low trust environment.

TradeLens was built on Hyperledger Fabric, a distributed ledger platform created by IBM that provides value-add functionality over standard blockchain concepts.  These capabilities include: a configurable combination of public and private “channels” that can be used to build a “network of networks”, a pluggable consensus model, and a flexible approach to implementing smart contracts.

## Could this be solved before blockchain? 

Real-time document access is not unique to blockchain. However, it is difficult to track changes made within a traditional database, while this capability is inherent within a blockchain based platform. Furthermore, if a previous entry is changed, it is easy to track where the change was made, increasing confidence in the stored documents.
Does more than one participant or organization need to update the data? Do the parties/organizations trust each other?

Each shipment can involve tens of organizations, over a hundred individuals, and several hundred information exchanges. Ensuring traceability across these many actors is vital and handled well by the historical ledger, improving collaboration across the industry. Shipping is inherently a low trust environment due to the variety of actors. The inherent cryptographic authentication and the strong tamper resistance of the blockchain makes audits more trustworthy. Furthermore, the blockchain’s distributive nature allowed all the organizations to participate in the platform without having to agree on any centralized authority. 

## Do entries need to be changed or updated? Do you need redundant copies of the data for auditing?

Entries would need to be changed and updated. However, due to the low-trust environment, the audit trail generated by these updates is beneficial despite the inefficiency. The blockchain’s ledger and redundant copies of the data worked to prevent willful data corruption and track the origin of incorrect data as any inconsistency would be caught due to the other nodes in the blockchain network.

## Are all entries public information?

TradeLens dealt with both public and commercial data, the latter of which was managed in two ways. Through its use of IBM’s Hyperledger Fabric blockchain technology, TradeLens allowed users to list parties that would need access to uploaded data, from which a sub-networks was created within the permissioned blockchain to restrict access to only those stakeholders. For some proprietary information such as invoices, the data was stored off chain and hashed. The hash allowed the document to be verified and traced – but the actual data did not need to be stored on chain. 

## Results

TradeLens was first launched in 2016, moved to general availability in 2018. It encountered certain implementation challenges – primarily in adoption. Certain participants didn’t have the technical capabilities or organizational infrastructure to run a node – in these cases, they would likely access the platform through an API that reached a node operating in the network. About 100 organizations participated at launch, and within its pilot it successfully decreased transit time, reduced operations time, and reduced the number of unnecessary inspections. TradeLens was the only successful deployment of an Enterprise Blockchain within a public supply chain network.

TradeLens is set to discontinue operations in the first quarter of 2023. TradeLens was regarded as a viable platform and technology, but according to Head of Business platforms at Maersk, “the need for full global industry collaboration has not been achieved”, and TradeLens’ limited deployment mean it was not able to reach commercial viability.
 
# References

- 101 Blockchains. (2020, June 29). When to use blockchain technology? 101 Blockchains. Retrieved December 5, 2022, from https://101blockchains.com/when-to-use-blockchain/ 
- Baiod, W., Light, J., & Mahanti, A. (2021). Blockchain Technology and its Applications Across Multiple Domains: A Survey. Journal of International Technology and Information Management, 29(4). Retrieved from https://scholarworks.lib.csusb.edu/jitim/vol29/iss4/4. 
- Berryhill, J., T. Bourgery and A. Hanson (2018), “Blockchains Unchained: Blockchain Technology and its Use in the Public Sector”, OECD Working Papers on Public Governance, No. 28, OECD Publishing, Paris. http://dx.doi.org/10.1787/3c32c429-en 
- Casino, F., Dasaklis, T. K., & Patsakis, C. (2019). A systematic literature review of blockchain-based applications: Current status, classification and open issues. Telematics and Informatics, 36, 55–81. https://doi.org/10.1016/j.tele.2018.11.006 
- Cecere, L. (2022, December 6). Tradelens discontinues operations. why you should care. Forbes. Retrieved December 20, 2022, from https://www.forbes.com/sites/loracecere/2022/12/05/tradelens-discontinues-operations-why-you-should-care/?sh=8e57d6d4cec5
- Clavin, J., Duan, S., Zhang, H., Janeja, V. P., Joshi, K. P., Yesha, Y., Erickson, L. C., & Li, J. D. (2020). Blockchains for government. Digital Government: Research and Practice, 1(3), 1–21. https://doi.org/10.1145/3427097 
- Di Francesco Maesa, D., & Mori, P. (2020). Blockchain 3.0 Applications survey. Journal of Parallel and Distributed Computing, 138, 99–114. https://doi.org/10.1016/j.jpdc.2019.12.019
- IBM. (n.d.). About Tradelens. TradeLens. Retrieved December 20, 2022, from https://www.tradelens.com/about
- Nair, R., Benjelloun, R., Waite, V., & Barry, K., BLOCKCHAIN FOR TRADE: SELECT CASE STUDIES AND LESSONS LEARNED (2018). United States Agency for International Development (USAID). Retrieved from https://pdf.usaid.gov/pdf_docs/PA00TKX9.pdf. 
- United States Government Accountability Office, Blockchain Emerging Technology Offers Benefits for Some Applications but Faces Challenges (2022). Retrieved from https://www.gao.gov/assets/gao-22-104625.pdf. 
- Why use blockchain and when it's better not to. PixelPlex. (2022, March 2). Retrieved December 5, 2022, from https://pixelplex.io/blog/why-use-blockchain-and-when-not-to/



