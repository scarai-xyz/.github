# SCAR AI

Don't trust the fix. Replay the attack.

AI agents now write smart-contract security fixes in minutes. SCAR checks whether a fix holds: we fork the chain one block before a real exploit, replay the attack against the fix, run the security and legitimate-use checks the fix was never shown, and return a verdict with a receipt anyone can re-run.

## What is here

- [evmpatch-env](https://github.com/scarai-xyz/evmpatch-env): the open checker. Four real incidents (MCAI on Ethereum, and GoldReserve, Bitallx and NGP on BNB Chain), each frozen one block before the attack, with hidden security and legitimate-use tests. Apache-2.0. Every CI run re-grades every committed control and fails if a hash moves.
- [scar-retrieval](https://github.com/scarai-xyz/scar-retrieval): earlier work. Sparse retrieval over smart-contract audit findings, with the training and evaluation code and the benchmark datasets.

## Evidence

- [48 receipts](https://scarai.xyz/receipts/): every test fix in the control suite, graded on frozen chain state and hashed. 26 block the exploit, and only 11 are complete repairs. Open any receipt for the checks, the patch and the command that re-runs it.
- [Revision review](https://scarai.xyz/revisions/): verdicts re-checked when the code changes, shown on four public changes to OpenZeppelin Contracts and Safe Smart Account. No affiliation with either project.
- [Cases](https://scarai.xyz/cases/): the four incidents, block by block.
- Datasets on Hugging Face: [scar-corpus](https://huggingface.co/datasets/Farseen0/scar-corpus), [scar-eval](https://huggingface.co/datasets/Farseen0/scar-eval), [scar-pairs](https://huggingface.co/datasets/Farseen0/scar-pairs), [scar-pairs-extended](https://huggingface.co/datasets/Farseen0/scar-pairs-extended).

## Talk to us

A case you want checked, a fix you want graded, or a question: open a thread in [Discussions](https://github.com/scarai-xyz/evmpatch-env/discussions), or write to farseen@scarai.xyz.
