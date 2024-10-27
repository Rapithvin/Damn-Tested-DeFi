## Usage

Each challenge is made up of:

- A prompt located in `src/<challenge-name>/README.md`.
- A set of contracts located in `src/<challenge-name>/`.
- A [Foundry test](https://book.getfoundry.sh/forge/tests) located in `test/<challenge-name>/<ChallengeName>.t.sol`.

To solve a challenge:

1. Read the challenge's prompt.
2. Uncover the flaw(s) in the challenge's smart contracts.
3. Code your solution in the corresponding test file.
4. Try your solution with `forge test --mp test/<challenge-name>/<ChallengeName>.t.sol`.

> In challenges that restrict the number of transactions, you might need to run the test with the `--isolate` flag.

If the test passes, you've solved the challenge!

Challenges may have more than one possible solution.