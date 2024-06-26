# Voting DApp

This project is a decentralized voting application built with ReactJS and Solidity. It uses smart contracts to ensure that only users with governance tokens can participate in the voting process.

Thw Solidity contract is for a voting system where voters can register, candidates can register, and voters can cast their votes for the registered candidates. The contract includes the following functionalities:

1. **Candidate registration**: Candidates can register with their personal details, and the contract checks if the candidate has already registered. The contract also checks if the number of candidates registered is less than the maximum limit of 3.
2. **Voter registration**: Voters can register with their personal details, and the contract checks if the voter has already registered. The contract also checks if the voter's age is at least 18.
3. **Voter and candidate verification**: The contract includes functions to verify if a voter or candidate has already registered.
4. **Voter list and candidate list**: The contract includes functions to retrieve the list of registered voters and candidates.
5. **Voting**: Voters can cast their votes for the registered candidates. The contract checks if the voter has already voted, if the voter has enough tokens to vote, if the voting period has started, if the number of candidates registered is 3, if the candidate ID is valid, and if the voter is a registered voter.
6. **Voting time**: The contract includes a function for the election commissioner to set the start and end times for the voting period.
7. **Voting status**: The contract includes a function to check the current status of the voting period.
8. **Result**: The contract includes a function for the election commissioner to announce the election result. The contract checks if at least one candidate has registered before announcing the result.
9. **Emergency**: The contract includes a function for the election commissioner to stop the voting process in case of an emergency.

The contract uses OpenZeppelin's SafeERC20 library to safely interact with the ERC20 token contract. The contract also includes several events to log important actions, such as candidate registration, voter registration, vote casting, voting period set, voting status updated, and election result announced.

## Features

* **Secure Voting:** Utilizes smart contracts to ensure tamper-proof voting results and token-based voting access.
* **Token-based Voting:** Requires users to hold governance tokens to participate in voting.
* **Intuitive User Interface:** Provides a user-friendly interface for registering, voting, and viewing results.

## Getting Started

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/SanskarDhyani98/Voting.git
   cd Voting/client
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

3. **Start the Development Server:**
   ```bash
   npm run dev
   ```
   This will start a development server and open the application in your browser.

## Usage

1. **Register as a Voter:**
   * Visit the registration page and provide your details.
   * Acquire governance tokens.

2. **Vote:**
   * Login to your account and navigate to the voting page.
   * Cast your votes.

3. **View Results:**
   * Once voting is complete, view the results on the results page.

## Architecture

* **Frontend:** ReactJS is used for building the user interface.
* **Backend:** Solidity smart contracts handle voting logic and token management.
* **Blockchain:** The application interacts with a blockchain network, such as Ethereum.

## Contribution

Contributions are welcome! If you'd like to contribute, please submit a pull request.

## License

This project is licensed under the MIT License.

## Acknowledgements

This project was inspired by the growing interest in decentralized voting and the potential of blockchain technology.

## Contact

If you have any questions or feedback, please feel free to contact Sanskar Dhyani at 
sanskardhyani98@gmail.com.
