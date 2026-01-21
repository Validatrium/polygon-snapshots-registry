# Polygon Snapshots Registry

This repository contains a list of public snapshots for polygon provided by different validators.

## How to Add Your Snapshot

1. Create a **fork** of this repository.
2. Copy the file `validators/template.json`  into a new file `validators/<your-validator-name>.json`
3. Fill in the following fields::
   - `validator`
   - `network name` (mainnet or testnet)
   - `bor.snapshot.block`
   - `bor.snapshot.url`
   - `bor.snapshot.checksum_url`
   - `bor.snapshot.size`
   - `bor.snapshot.compression`
   - `bor.snapshot.updated_at` (UTC, ISO8601 format)
   - `heimdall.snapshot.block`
   - `heimdall.snapshot.url`
   - `heimdall.snapshot.checksum_url`
   - `heimdall.snapshot.size`
   - `heimdall.snapshot.compression`
   - `heimdall.snapshot.updated_at` (UTC, ISO8601 format)

4. Commit your changes `git commit` and `push` them to your fork. 
5. Open a **Pull Request** to this repository.

## How to Update Your Snapshot

1. Update the fields in your file `validators/<your-validator-name>.json`:
   - `bor.snapshot.block`
   - `bor.snapshot.url`
   - `bor.snapshot.checksum_url`
   - `bor.snapshot.size`
   - `bor.snapshot.updated_at`
   - `heimdall.snapshot.block`
   - `heimdall.snapshot.url`
   - `heimdall.snapshot.checksum_url`
   - `heimdall.snapshot.size`
   - `heimdall.snapshot.updated_at`

2. Create a new Pull Request with the updated file.

Once the PR is merged, our Discord bot will automatically pull the updated data and announce the new snapshot
