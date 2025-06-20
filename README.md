# opensouthcode25-plain-text-accounting

This repo contains all the examples used in my OpenSouthCode 2025 talk on plain text accounting.

```bash
# Overview

## Basics
hledger -f ./2025.ledger bs --tree --monthly --percent
# Income Statement (is) / Balance Sheet (bs)
# not:"assets:property:home" not:"liabilities:mortgage"
# --forecast

# Adding Transactions
## Manually (copilot, etc)
## Add command
## Importing transactions from CSV
hledger -f bankA.csv print 

# Visualization (web/ui)

# Non-native tools I use
## VScode Extension
# https://marketplace.visualstudio.com/items?itemName=dgzlopes.ledger-highlight

## Formatter (https://github.com/mondeja/hledger-fmt)
./hledger-fmt --fix 2025.ledger

## Puffin (https://github.com/siddhantac/puffin)
./puffin --cfg puffin.config.json

# hledger-tools
# https://github.com/dgzlopes/hledger-tools
# add / import / ask
```