How to run the Paying Guest Accommodation System (PGAS) Project
1. Download the  zip file

2. Extract the file and copy pgas folder

3.Paste inside root directory(for xampp xampp/htdocs, for wamp wamp/www, for lamp var/www/html)

4. Open PHPMyAdmin (http://localhost/phpmyadmin)

5. Create a database with name pgasdb

6. Import pgasdb.sql file(given inside the zip package in SQL file folder)

7.Run the script http://localhost/pgas (frontend)

8. For owner panel

http://localhost/pgas /owner/login.php  (owner panel)

9. For admin panel

http://localhost/pgas /admin  (admin panel)

Credential for admin panel :

Username: admin Password: Test@123

Credential for user panel :

Username: testuser@gmail.com Password: Test@123

Credential for owner panel :

Username: pgtest@gmail.com Password: Test@123




Below is a detailed list of features in your project along with explanations of how each one benefits the system. You can use this comprehensive overview in your research paper:

1. Decentralized Blockchain Architecture
Feature:
The project implements a blockchain that records transactions in immutable blocks.
Benefit:
Security & Transparency: Each block is cryptographically linked to its predecessor, making data tampering nearly impossible.
Decentralization: Eliminates a single point of failure and builds trust among participants (e.g., farmers, validators, customers).
2. Validator Pool with Staking Mechanism
Feature:
Validators (e.g., quality check experts) must stake a fixed amount of tokens to participate. The system tracks validator reputation, assigned transactions, and queue capacity.
Benefit:
Incentive & Accountability: Staking ensures validators have a financial commitment, reducing malicious behavior.
Reputation System: Helps in selecting the most reliable validators, improving decision accuracy.
3. Dynamic Validator Assignment and Queue Management
Feature:
Transactions are automatically assigned to multiple validators based on their reputation and current queue capacity. If a validator’s queue is full, the transaction is assigned to the next available validator.
Benefit:
Load Balancing: Prevents any single validator from being overwhelmed and ensures prompt processing of transactions.
Fair Distribution: Improves overall system performance and responsiveness.
4. Transaction Pool and Voting Mechanism
Feature:
A transaction pool holds produce submissions until they receive validations. Transactions require at least 50% of assigned validator approvals (or an AI override) to be finalized.
Benefit:
Consensus-Based Approval: Ensures only high-quality and agreed-upon transactions are added to the blockchain.
Robust Quality Assurance: Reduces the risk of fraudulent or low-quality produce entering the system.
5. AI-Based Quality Check Fallback
Feature:
If validator votes do not reach the required threshold, an AI quality check analyzes IoT sensor data and physical sample data to make a final decision.
Benefit:
Enhanced Reliability: Provides a backup when human validation is inconclusive, ensuring continuity of operations.
Objective Assessment: The AI algorithm can detect patterns and discrepancies that might be missed by human validators.
6. Integration with IPFS for Off-Chain Data Storage
Feature:
IoT sensor data and physical sample data are uploaded to IPFS, and only their hash references are stored in transactions.
Benefit:
Scalability: Offloads large data from the blockchain, keeping it lightweight and efficient.
Data Integrity: IPFS ensures decentralized, immutable storage of critical data for later verification.
7. Digital Signature & Cryptography
Feature:
Every transaction is signed using Elliptic Curve (EC) cryptography, and signatures are verified to ensure authenticity.
Benefit:
Security: Prevents unauthorized transactions and ensures that only legitimate parties can initiate actions.
Trust: Strengthens the overall integrity of the system.
8. Automatic Mining Trigger
Feature:
A background process periodically checks the transaction pool and automatically mines a block when approved transactions are available.
Benefit:
Efficiency: Reduces manual intervention and speeds up the inclusion of valid transactions into the blockchain.
Real-Time Updates: Ensures the blockchain is constantly updated, maintaining system synchronicity.
9. Merkle Tree Verification
Feature:
A Merkle tree is built from block hashes to verify the integrity of the entire blockchain.
Benefit:
Data Integrity: Quickly verifies that transactions within a block haven’t been tampered with.
Scalability: Efficiently handles a large number of transactions with minimal overhead.
10. RESTful API Endpoints
Feature:
The system exposes multiple REST endpoints (for registration, wallet info, produce submission, validation, blockchain retrieval, etc.) to interact with the network.
Benefit:
Interoperability: Allows different users (farmers, validators, customers) to interact with the blockchain seamlessly.
Accessibility: Facilitates integration with web and mobile applications, enhancing user experience.
11. State Synchronization via Pub/Sub Mechanism
Feature:
A Pub/Sub (publish/subscribe) system disseminates updates (new transactions, blockchain changes, validator pool updates) across all nodes in real time.
Benefit:
Consistency: Ensures all network participants have the latest state, improving consensus and reducing data discrepancies.
Decentralization: Promotes robust communication in a distributed environment.
12. Robust Data Rehydration and Object Methods Preservation
Feature:
A fromJSON method ensures that transactions retrieved as plain objects are rehydrated into full instances with methods intact.
Benefit:
Reliability: Prevents runtime errors and ensures that object methods (like updateValidation and finalizeTransaction) work as expected.
Summary of Benefits
Security & Integrity:
Cryptographic signatures, immutable blockchain structure, and Merkle tree verification all work together to secure the data.

Decentralized Trust:
A validator pool with staking and reputation systems incentivizes accurate validations and reduces fraudulent behavior.

Efficient Data Handling:
Offloading large files to IPFS and using a transaction pool for pending submissions help keep the system efficient and scalable.

Resilient Decision-Making:
The combination of validator consensus and AI-based fallback ensures that only high-quality produce data is approved and recorded.

User-Centric Interface:
RESTful APIs provide an accessible and interoperable interface, allowing various stakeholders (farmers, validators, customers) to interact with the system seamlessly.

Each feature not only strengthens the technical robustness of your blockchain but also addresses key challenges in agricultural supply chains—such as ensuring produce quality, transparency, and trust in a decentralized environment. These benefits can be directly highlighted in your research paper to demonstrate how the system enhances efficiency, security, and trust in the agriculture sector.

Let me know if you need any further details or adjustments!
